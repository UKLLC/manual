# File 2 specification

## Formatting of attribute datasets (File 2s)

The UK LLC default is for LPS to provide datasets as either **STATA or SPSS files** with variable and value labelling in place. Where an LPS does not routinely store data as STATA or SPSS then we ask that you create **.csv data** and **metadata files** to the structure detailed in **Tables 4 to 6** below.  

> **An example File 2 with .csv data and metadata files can be found downloaded from [here](../downloads/download_intro.md#file-2-downloads).**  

File 2s should have the same structure as the existing LPS' file structure and documentation – they can have long or wide format and can contain hierarchies. Additional IDs (e.g. indicating an event) can be included, but these must not include externally meaningful IDs (e.g. NHS ID).

<span style="color:teal">**The variable names must be the same as the names used in LPS documentation.**  

The content and structure of a File 2 must have corresponding documentation as described [**here**](../file2s/file2_documentation.md).  

### Table 4: File 2 attribute data .csv specification - only relevant if you do not store data in STATA or SPSS files.  
|Field Name | Data Type |
|---|---|
| STUDY_ID | varchar(50) (Unique)
| Timestampvariable | Variable indicating the date/time when data were collected |
| ........... | LPS information | 

Please separate variable and value labels into **two .csv metadata** files as outlined in Tables 5 & 6 below.
<br>  

### Table 5: File 2 variable label .csv specification - only relevant if you do not store data in STATA or SPSS files.
|Field Name | Data Type | Description |
|---|---|---|
| Dataset_Name | varchar(50) | The full and exact name you give the File 2 (see '[File 2 naming conventions](../file2s/file2_naming.md)') but do not include the file type postscript (e.g. do not include the .csv element). |
| Variable_Name | varchar(50) | The full and exact name that you use in your documentation for every variable included in the dataset. |
| Variable_Label | varchar(255) | The full and complete label that you use in your documentation for every variable included in the dataset. |  

### Table 6: File 2 value label .csv specification - only relevant if you do not store data in STATA or SPSS files. 
|Field Name | Data Type | Description |
|---|---|---|
| Dataset_Name | varchar(50) | The full and exact name you give the File 2 (see '[File 2 naming conventions](../file2s/file2_naming.md)') but do not include the file type postscript (e.g. do not include the .csv element). |
| Variable_Name | varchar(50) | The full and exact name that you use in your documentation for every variable included in the dataset. |
| Value_Value | varchar(255) | The underlying (un-labelled) value (e.g. 1, 2). |
| Value_Label | varchar(255) | The full and complete label that you use in your documentation (e.g. Male, Female). | 

<br>

> **The File 2 naming conventions are on the next page**

