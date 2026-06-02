# File 2 naming conventions
>Last modified: 02 Jun 2026
<div style="background-color: rgba(0, 178, 169, 0.3); padding: 5px; border-radius: 5px;"><strong>How to name File 2s and the accompanying metadata.</strong></div>

## Attribute data files should be named as:

`<UK LLC Study Code>_<dataset_name>_v<version>_<YYYYMMDD>`  

Where:
| | |
|---|---|
`<UK LLC Study Code>` | See [Appendix C](../appendix/c_study_codes.md) for the standardised names for each study  |
| `<dataset_name>` | The dataset name, as described in LPS documentation  |
| `<version>` | Corresponds to a numeric versioning value as sequenced by the LPS in order of deposit<br> to UK LLC. Version should be provided as a 4-digit number: v0001, v0002, etc. |
| `<YYYYMMDD>` | Should be the day that the file was created and should match the date recorded in the<br> File 2 documentation. (If files are batched and sent over two or more days, they should<br> all be named with the date of the first file in the batch.)

<span style="color:teal"><strong>e.g. EXCEED_COVIDWAVE1_v0001_20210514.dta</strong>  
<br>

## Metadata files (for LPS providing .csv files) should be named as:  

### File 2 Variable Labels ([see Table 5](../file2s/file2_spec.md#table-5-file-2-variable-label-csv-specification---only-relevant-if-you-do-not-store-data-in-stata-or-spss-files))  

`<UK LLC Study Code>_<dataset_name>_v<version>_<description>_< YYYYMMDD>`  

<span style="color:teal"><strong>e.g. EXCEED_COVIDWAVE1_v0001_description_20210514.csv</strong>  

### File 2 Value Labels ([see Table 6](../file2s/file2_spec.md#table-6-file-2-value-label-csv-specification---only-relevant-if-you-do-not-store-data-in-stata-or-spss-files))

`<UK LLC Study Code>_<dataset_name>_v<version>_<values>_< YYYYMMDD>`  

<span style="color:teal"><strong>e.g. EXCEED_COVIDWAVE1_v0001_values_20210514.csv</strong>  
<br>

## File 2 documentation should be named as: 
`<UK LLC Study Code>_<file2documentation>_v<version>_<version_dateYYYYMMDD>`  

<span style="color:teal"><strong>e.g. EXCEED_file2documentation_v0002_20211119.xls</strong>
<br>

<aside class="admonition note"><p class="admonition-title">More information on File 2 documentation in on the next page.</p></aside>