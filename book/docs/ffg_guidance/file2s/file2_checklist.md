# Attribute Data File (File 2) Checklist

You should submit attribute data (a File 2) and accompanying documentation each time new or updated datasets are deposited into the UK LLC TRE.  

File 2s contain a STUDY_ID and de-identified LPS data. We ask that LPS provide File 2s containing **logical datasets** which can be shared with researchers as full datasets rather than having to be minimised further. For example:  
• A questionnaire collected at one timepoint  
• A file of core SES/demographic indicators and timepoints  
• Data collection assessments during a home visit  
• Assayed biosamples from COVID-19 serology tests  
• Chapters from questionnaires, or themed data pulled from across chapters of questionnaires.  

Datasets are created at the LPS’ discretion but should be as meaningful as possible to a research user. If in doubt, please get in touch to discuss this: support@ukllc.ac.uk.

> When preparing a File 2, please work carefully through the list below.  

## Attribute data file (File 2) requirements

**Participant data**
| | |
|:---:|---|
| 01 | Include STUDY_ID in each File 2 (the same as for each individual as used in File 1) | 
| 02 | Include a participant-level date of data collection (a 'timestamp' variable). This should be set for the dataset if all data were collected at the same time, or per variable if the data come from multiple timepoints. Where practical and relevant, the timestamp could include minutes and seconds. |
| 03 | Ensure the file does not contain direct identifiers such as name or postcode. Some indirect identifiers and pseudo-identifiers can be included, because they have strong research utility (e.g. gender, ethnicity, age). The LPS should ensure that these are processed to their local disclosure control standards. |
| 04 | Structure the data in logical datasets relating to data collection assessments: these should be based on a collection phase (e.g. a visit or questionnaire) and should not need further sub-division. | 
| 05 | Ensure none of the datasets exceed 1,024 variables. (Files with more than 1,024 variables cannot be processed.) | 
| 06 | DO NOT include any free text variables. Note: processed or derived outputs from these variables are acceptable. | 
| 07 | DO NOT include any geographical units (e.g. LSOAs, postcodes, partial postcodes, encrypted geo markers, IMD) or any strong proxies for location e.g. 'assessment centre name' where this contains location information smaller than region. |

**Specification and transfer of File 2s and documentation**  
| | |
|:---:|---|
| 08 | Either prepare the File 2 in STATA/SPSS with full labelling<br>Or use the .csv specification, providing both attribute data and metadata <span style="color:red">(see Tables 4, 5 & 6 below for further details). |
| 09 | Adhere <strong>exactly</strong> to the File 2 specification detailed in <span style="color:red">Section 3.1 below. |
| 10 | Name the file as detailed in <span style="color:red">Section 3.1.2 using the agreed UK LLC study code (see Appendix C). |
| 11 | If splitting one attribute file into several parts, ensure all files names contain the same date and that the separate 'batches' are numbered consecutively. |
| 12 | Send the File 2 to Swansea University via the secure file upload portal. See '[File Transfer to UK LLC](#file-2-transfer-to-uk-llc-previously-section-34)' (below) for upload instructions. |
| 13 | Complete the <span style="color:red">File 2 Documentation Template.xlsx[link to download] (further details in Section 3.2 below). |
| 14 | Send the completed File 2 documentation template to both Swansea University (via the secure link) and the UK LLC Data Team (support@ukllc.ac.uk). |  

### File 2 Transfer to UK LLC <span style="color:red">(previously Section 3.4)</span>
UK LLC will ensure an LPS-specific link is sent from Swansea to each LPS Data Manager, which will provide a **one-way file drop** to Swansea. This service uses **Owncloud**, which is a Swansea-hosted client-server software and will allow direct upload of files for the Swansea team to process and load into the UK LLC TRE.  

**If this is not feasible for your LPS, please contact the UK LLC Data Team via [support@ukllc.ac.uk](mailto:support@ukllc.ac.uk) to discuss alternative arrangements.**