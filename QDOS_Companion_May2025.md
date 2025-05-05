# QDOS Companion Amendments.

**NOTE**: Where I use a page number in the following, I'm referring to the page in the ODT file, not the page numbers as per the QDOS Companion itself.


## Unknowns and Queries

Search for orange highlighted text which indicates areas I'm not sure of or OCR problems I don't have my book to correct.


## Spelling Errors

These have been corrected where obvious, without noting the locations or highlighting in any way.


## Search Replace Changes Made

Select Match case and Whole word only. Do not Replace All, check individually!

* ODOS -> QDOS
* AI -> A1
* AS -> A5
* IHe -> The
* OL -> QL
* DI -> D1
* Al -> A1
* PRINC -> JB.PRINC
* SERIC -> SER1C
* AQ -> A0
* $O -> $0
* DO -> D0

## Additions

### Page 21: MT.ALCHP 

* D2.L Owner Job ID missing from input registers. 
* Updated D1.L in return registers to note the figure included the bytes for the heap header.

### Page 27: MT.CJOB

* Input register A1.L updated to add "or 0", for the input registers.
* Input register D3.L updated. It said "code space" but should be "data space" required. 

### Page 35: MT.FREE

* D1.L removed from the input parameters in the table as there are no input parameters.

### Page 49: IO.OPEN

* It's possible that A1 is not preserved by the trap call. The SMSQ manual shows it as corrupted. (Highlighted but unchanged in text.)

### Page 51: IO.FORMT

* It's possible that A1 is not preserved by the trap call. The SMSQ manual shows it as corrupted. (Highlighted but unchanged in text.)

### Page 60: IO.SBYTE

* Deleted the text "high word: cursor position" from D1.B input register. Replaced with "Byte to be sent".

### Page 61: IO.SSTRG

* Deleted the text "high word: cursor position" from D1.B input register. Replaced with "Number of bytes to be sent".

### Page 81: SD.PXENQ

* It's possible that D1 is not preserved by the trap call. The SMSQ manual shows it as corrupted. (Highlighted but unchanged in text.)

### Page 82: SD.CHENQ

* It's possible that D1 is not preserved by the trap call. The SMSQ manual shows it as corrupted. (Highlighted but unchanged in text.)

### Page 83: SD.BORDR

* It's possible that A1 is not preserved by the trap call. The SMSQ manual shows it as corrupted. (Highlighted but unchanged in text.)

### Page 84: SD.WDEF

* Input parameter A1.L is not listed. It points to the base of the definition block for the window. (Added)

### Page 114: MD.SECTR

* Output parameter A4.L is listed as corrupted. This register is not mentioned in the latest QDOS/SMSQ manual. I have not highlighted it, but I don't know if it's corrupted or not, so probably best to leave it in?

### Page 115: MD.READ

* Output parameter A4.L is listed as corrupted. This register is not mentioned in the latest QDOS/SMSQ manual. I have not highlighted it, but I don't know if it's corrupted or not, so probably best to leave it in?

### Page 116: MD.VERIN

* Output parameter A4.L is listed as corrupted. This register is not mentioned in the latest QDOS/SMSQ manual. I have not highlighted it, but I don't know if it's corrupted or not, so probably best to leave it in?

### Page 117: MD.WRITE

* Output parameter A4.L is listed as corrupted. This register is not mentioned in the latest QDOS/SMSQ manual. I have not highlighted it, but I don't know if it's corrupted or not, so probably best to leave it in?

### Page 132: MT.SCLCK

* Entry register D1.L (Time in seconds) was actually named as A1.L. Edited.

### Page 137: Code for D4=D1*D0 onwards

* The code in the operand column is missing for the bottom two code chunks on the page.

### Page 141: UT.MINT

* Input parameter A0.L, the channel ID was missing from the table. Added.
* A2 and A3 are flagged as being corrupted, but the latest QDOS manual says preserved. Highlighted.

### Page 142: CN.FTOD/CN.ITOD

* A2 and A3 are flagged as being preserved, but the latest QDOS manual says corrupted. Highlighted.

### Page 143: Various convert to ASCII vectors

* D1, D2, D3 and A2 are flagged as being preserved, but the latest QDOS manual says corrupted. Highlighted.
* D7 is flagged as preserved but is not mentioned in the input parameters or in the latest QDOS manual. Left untouched.

### Page 144: CN.DTOF/CN.DTOI

* D7.L, input register updated to mention that it can be zero.
* D3, output register is marked as preserved but the QDOS manual says corrupted.

### Page 145: Various convert from ASCII vectors 

* D3, output register is marked as preserved but the QDOS manual says corrupted.

### Page 148: UT.UNLMK

* Output register A1 is updated according to the latest QDOS manual. (Highlighted)

### Page 149: UT.CSTR

* A6.L missing from input registers. Added.

### Page 151: Figure 8.1

* The various BV.XXX variables were named BY.XXX. Edited.

### Page 153: Text problem

* The text in the second paragraph, below the table at the top of the page, line three, reads "(Note that there are (or $20(A6) to $24(A6))," this makes no sense. Highlightes but uncorrected.

Page 154: BP.INIT

* Output register D2 is marked as preserved but the QDOS manual says corrupted.
* Output register D3 is marked as corrupted but the QDOS manual says preserved.

### Page 158: BV.CHRIX

* A1.L on inout, was missing from the table. Added.

### Page 159: Various CA.GTxxx vectors

* It looks like output registers A0 and A1 are switched around. A0 is listed as being the updated top of the maths stack and A1 is listed as corrupted. It's the other way around. Changed.

### Page 161: BP.LET

* Input register A1.L missing from table. Added.

### Page 161: Channel table

* I'm not convinced that CH.CCPY and CH.CCPX are the names for the current graphics y and x coordinates but I don't have a QDOS manual (only SMSQ) to check with. Highlighted in case they need changing.

### Page 163: Some Examples.

* 5 lines up from the bottom of the page there's the text "CAT V". I suspect the V should be a digit? "Cat 1" perhaps?

### Page 170: Text problem.

* The second last paragraph on the page doesn't end sensibly. Some text appears missing. I've highlighted the paragraph.


