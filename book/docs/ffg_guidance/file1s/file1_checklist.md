# Identifiable Data File (File 1) Checklist

Updated identifiers (File 1s) and accompanying documentation should be submitted **each quarter**. The schedule and deadlines for File 1 submission can be found <span style= "color:red">**here**. 

If no updates are required, please send an email to support@ukllc.ac.uk to confirm this.

> When preparing a File 1, please work carefully through the list below.  

## File 1 (identifiers) requirements:  
<details>
<summary>1. Set up an account with NHS Digital Health & Care Wales (DCHW)</summary>  
A secure electronic data transfer facility at NHS DHCW is available for uploading participant identifiers. NHS DHCW has been informed of all LPS and data managers’ details, so is expecting LPS Data Managers to be in contact to set-up accounts.
To set up an account contact <strong>pdit@wales.nhs.uk</strong> and request an account for UK LLC. In this email please specify:  

* Your name  
* Your institution, including centre, e.g. Joe Blogs, Centre for XYZ, University of Nowhere.
* The datasets you are uploading – this is the LPS title.
* That you would like to set up a UK LLC account.  

<strong><span style= "color:teal">Do NOT send File 1s to the UK LLC Data Team or Swansea University.  
<span style= "color:teal">NEVER send File 1s via e-mail as it NOT secure for transferring potentially sensitive personal information.</strong>
</details>

<details><summary>2. Identify participants to be deposited in the UK LLC TRE</summary>

* Only those individuals where there is a legal basis for their inclusion in the UK LLC TRE are provided.  
* Please include as many participants as possible to minimise bias.  
*  It is permitted to send records of deceased participants.  

<strong><span style= "color:teal">Participants can be included in the UK LLC TRE on the basis that only their LPS data are accessed by researchers and, optionally, that their identifiers can be sent for linkage to NHS records, UK Government records, or place-based data providers/modellers for geocoding. Please discuss any other filtering with us so we can understand the denominator provided.</strong>
</details>  

<details><summary>3. If you are using NHS IDs supplied by NHS England, then the use of these with UK LLC <strong>MUST be made explicit and clear in your DSA</strong> with NHS England.</summary>  

More information about this is provided in [**Appendix B**](../appendix/b_nhs_dsas.md).
</details>

<details><summary>4. Produce one file of identifiers (a File 1) per LPS.</summary>  

You should update this periodically (to add new participants, to amend permission flags or to add address information for geocoding). You will be asked every quarter to send an updated File 1 to NHS DHCW to reflect the latest withdrawals of consent and update of permission status flags.  
However, if there are NO changes to the content of a File 1, then there is NO requirement to send a File 1, but please email [support@ukllc.ac.uk](mailto:support@ukllc.ac.uk) to confirm this.
</details>

<details><summary>5. Include all participants’ identifiers, with historical variations where available</summary>  

* Once a participant has been included in a File 1 <strong>they should NEVER be removed</strong> from a successive File 1, i.e. the number of rows in File 1 updates should only ever increase or remain stable.  
* Make sure to retain a 'Current Row' with a STUDY_ID for ALL participants ever included in UK LLC. Where a participant’s status has changed, please create a new row marked 'C' (current) and change the 'row_status' on the old record to 'H' (historical). For more details refer to the [**File 1 specifications**](file1_spec.md).  
* <strong><span style= "color:teal">Deleting previously listed participants in a File 1 update will NOT stop their data from flowing – you MUST use permission flags – see point 6 below</strong>.  
* If participants have died between File 1 updates, please continue to allow participants’ data to flow to the UK LLC TRE, unless doing so is in violation of your LPS protocol. Please note that UK LLC does not ask LPS for a status flag, and mortality data comes from linked mortality records where available.
</details>  

<details><summary>6. Set the participant permission flags</summary>  

* Ensure that the permission flags reflect the LPS participants’ wishes and current status. If a participant withdraws from your LPS or withdraws their consent to share data with UK LLC, <strong>set their UK LLC status to 0</strong> in the 'Current' row. If a participant objects to NHS linkages, ensure that their <strong>NHS flags are set to 0</strong>.
* Set permission flags to '1' for all NHS linkages unless there is a specific participant- or LPS-level reason for not doing this.
* Permission flags should only be populated for the CURRENT row of information.  

<span style="color:teal">**A major challenge with linkage is being able to infer whether a 'null' result (i.e. no linked records) is due to the participant not being ill and not seeking any health care, or a null return due to the participant’s care record not being linked. Linking across the four nations’ NHS allows us to reduce uncertainty over this and capture health records during spells of residence in different nations (e.g. a spell living in Scotland between two waves of data collection based on home interviews in England), complex living arrangements (students, separated families), working arrangements, help-seeking across borders and whilst on holiday.**
</details>

<details>
<summary>7. Adhere exactly to the File 1 specification.
</summary>  

This is outlined on the [next page](../file1s/file1_spec.md) 
</details>

<details><summary>8. Follow the File 1 naming convention</summary>  
The naming convention is as follows:  

    <UK LLC Study Code>_<FILE1>_v<version>_<YYYYMMDD>  
Where:  
* UK LLC Study Code: [see Appendix C](../appendix/c_study_codes.md)
* version: Corresponds to a numeric versioning value as sequenced by the LPS in order of deposit to NHS DHCW
* YYYYMMDD: The date should be the day that the file was created.

<span style="color:teal">e.g. EXCEED_FILE1_v1_20210514.csv</span>

File 1 updates should follow the File 1 naming convention, with each update given a new sequential version number and date. Clearly label versions of new files using file naming convention above.
</details>  

<details><summary>9. Retain all variables and use the exact variable names, in the same order as the <b>File 1 formatting table</b></summary>  

Do this even when data are absent for some variables. This is critical for the linkage process. The File 1 formatting table is on the [**next page**](../file1s/file1_format_table.md).
</details>  

<details><summary>10. Use the UK LLC 'File 1 Checker' programme to confirm that the file is formatted correctly.</summary>  

* The File 1 Checker can be downloaded from Github: https://github.com/UKLLC/File-Checker  
* It is a tool for LPS Data Managers to check that the contents of a File 1 are in line with the requirements set out in this guide.  
* The checker verifies that field names and values are of expected syntax and data type. It makes no judgment on the contents of the files other than their legality under formatting rules.  
* All File 1s MUST be cleared through the checker before being sent to DHCW.

<span style="color:teal"><strong>For details on how to use the 'File 1 Checker programme', use the <span style="color:red">File 1 Checker User Guide</strong>.
</details>  

<details><summary>11. Send the correctly formatted attribute data to NHS DHCW following the process sent out in step 1 above</summary>  

* Make sure to double check the date format to avoid inconsistent formats and follow the specifications in the [**File 1 specifications**](file1_spec.md). 
* <span style="color:teal"><strong>DO NOT SEND THE FILE 1 TO ANY OTHER ORGANISATION</span></strong>
</details>

<details><summary>12. Send the 'File 1 checker' output (File1_doc.json) to the UK LLC Data Team (<b>support@ukllc.ac.uk</b>)</summary>  

* The File 1 documentation enables UK LLC and research users to understand the sample provided by each LPS and how it relates to the LPS headline denominator.
* This step is important, because without this information it will be difficult for analysts to consider the risk of potential bias and issues relating to generalisability.
</details>

<details><summary>13. Retain a copy of each File 1 for potential audit purposes</summary>
</details>

<br>

<span style="color:teal"><strong>The File 1 specification is outlined on the next [page](../file1s/file1_spec.md)