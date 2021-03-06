# Summary
Scripts for processing & manipulating data in DSI Studio 

```createBfilesFromBtable.m```
	Creates separate bvec and bval files from single b-table saved from DSI Studio

```dsiStudioBatchRecodeDicom.sh```
	Recode subject DICOM files by sequence. Required if program cannot read raw data (e.g. extension is .v2 DICOM)
	Function will overwrite and rename raw data so perform only on a copy!!

```dsiStudioBatchReconstruct.sh```
	Reconstruct raw diffusion data into DSI Studio source file (.src.gz) 
	Subject ID and reconstruction method are required flags

```dsiStudioExportAtlas.sh```
	Exports diffusion metrics for regions within a given atlas
	Check DSI Studio install for case-sensitive atlas name
        Subject ID and atlas name are required flags

```dsiStudioText2CSV.m```
	Reads in text files saved from DSI Studio ROI information export
	Concatenates into single CSV for human-readable computation & manipulation
