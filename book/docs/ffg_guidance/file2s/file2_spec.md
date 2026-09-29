# File 2 specification
>Last modified: 28 Sep 2026
<div style="background-color: rgba(0, 178, 169, 0.3); padding: 5px; border-radius: 5px;"><strong>Formatting of attribute datasets (File 2s).</strong></div>  
<br>  

The UK LLC default is for LPS to provide datasets as either **STATA or SPSS files** with variable and value labelling in place. Where an LPS does not routinely store data as STATA or SPSS then we ask that you create **.csv data** and **metadata files** to the structure detailed in **Tables 1 - 3** below.  

File 2s should have the same structure as the existing LPS' file structure and documentation – they can have long or wide format and can contain hierarchies. Additional IDs (e.g. indicating an event) can be included, but these must not include externally meaningful IDs (e.g. NHS ID).

<aside class="admonition note"><p class="admonition-title">The variable names must be the same as the names used in LPS documentation.</p></aside>

<br>

<big>**Table 1: File 2 attribute data .csv specification</big> (only relevant if you do not store data in STATA or SPSS files).**  
|Field Name | Data Type |
|---|---|
| STUDY_ID | varchar(50) (Unique)
| Timestampvariable | Variable indicating the date/time when data were collected |
| ........... | LPS information | 

Please separate variable and value labels into **two .csv metadata** files as outlined in Tables 2 & 3 below.  
<br>  
  
<big>**Table 2: File 2 variable label .csv specification</big> (only relevant if you do not store data in STATA or SPSS files).**
|Field Name | Data Type | Description |
|---|---|---|
| Dataset_Name | varchar(50) | The full and exact name you give the File 2 (see '[File 2 naming conventions](../file2s/file2_naming.md)') but do not include the file type postscript (e.g. do not include the .csv element). |
| Variable_Name | varchar(50) | The full and exact name that you use in your documentation for every variable included in the dataset. |
| Variable_Label | varchar(255) | The full and complete label that you use in your documentation for every variable included in the dataset. |   
<br>

<big>**Table 3: File 2 value label .csv specification</big> (only relevant if you do not store data in STATA or SPSS files).** 
|Field Name | Data Type | Description |
|---|---|---|
| Dataset_Name | varchar(50) | The full and exact name you give the File 2 (see '[File 2 naming conventions](../file2s/file2_naming.md)') but do not include the file type postscript (e.g. do not include the .csv element). |
| Variable_Name | varchar(50) | The full and exact name that you use in your documentation for every variable included in the dataset. |
| Value_Value | varchar(255) | The underlying (un-labelled) value (e.g. 1, 2). |
| Value_Label | varchar(255) | The full and complete label that you use in your documentation (e.g. Male, Female). | 

<br>

> **The File 2 naming conventions are on the next page**

