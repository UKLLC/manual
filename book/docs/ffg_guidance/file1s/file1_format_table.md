# File Formatting Table

> File 1 formatting specification (multiple rows per individual)
<br> 

>You must use the Field Names in the table below and File Names **MUST** have underscores between words.

| <small>Order | <small>Field Name | <small>Data Type | <small>Description & values | 
|---:|---|---|---|
| 1<br><br><br><br> | <small>STUDY_ID<br><br><br><br> | varchar(50)<br><br><br><br> | Unique per participant * Relate to the same person when used in File 2 * Same for each row of data for each individual * Same for each individual across subsequent File 1s. <br><details><summary>Explanation</summary>Unique LPS-generated identifier (also to feature in 'File 2' attribute data file).|
| 2<br><br><br> | <small>ROW_STATUS<br><br><br> | char(1)<br><br><br> | C = Current<br>H = Historical/Alternative<br><details><summary>Explanation</summary>Indicates whether the row of information per participant is the ‘current’ row of information or a row containing historical or alternative values. | 
| 3<br><br><br><br><br><br><br> | <small>NHS_NUMBER<br><br><br><br><br><br><br> | varchar(10)<br><br><br><br><br><br><br> | Preferrably new NHS ID format, but old NHS ID is preferred to no NHS ID * Where LPS have encrypted 'Community Health Index' (CHI) number leave this null and instead populate NHS_S_Study_Number (field 22) with encrypted CHI * Include each known NHS ID as a separate row of information. The NHS ID which is likely to be most accurate should be included in the 'current' row. Leave null if not known or if inclusion is not permitted by your DSA. <details><summary>Explanation</summary> NHS number, formatted with no spaces. This should only be provided if the LPS’s DSA with NHSE permits onward sharing of NHS IDs. See [Appendix B](../appendix/b_nhs_dsas.md) for more information. |  
| 4<br><br> | <small>SURNAME<br><br> | varchar(255)<br><br> | Provide current name in 'current' row<br>Provide previous name(s) in separate rows of historical data |
| 5<br><br> | <small>FORENAME<br><br> | varchar(255)<br><br> | Provide current name in 'current' row<br>Provide previous or alternative forename(s) in separate rows of historical data |
| 6 | <small>MIDDLENAMES | varchar(255) | Space delimited middle name(s) | 
| 7<br><br><br><br> | <small>ADDRESS_1<br><br><br><br> | varchar(255)<br><br><br><br> | First line of address. <br>Provide current value in 'current' row <br>Provide previous address data (all address fields, postcodes and start/end dates) as separate rows of historical data |
| 8 | <small>ADDRESS_2 | varchar(255) | Second line of address |
| 9 | <small>ADDRESS_3 | varchar(255) | Third line of address (where available) |
| 10 | <small>ADDRESS_4 | varchar(255) | Fourth line of address (where available) |
| 11 | <small>ADDRESS_5 | varchar(255) | Fifth line of address (where available) | 
| 12<br><br><br><br> | <small>POSTCODE<br><br><br><br> | varchar(8)<br><br><br><br> | Postcode, where possible in formal space separated format, i.e.<br>4 & 3 = "YYYY ZZZ" <br>3 & 3 = "YYY ZZZ"<br>2 & 3 = "YY ZZZ"  | 
| 13<br><br><br><br> | <small>ADDRESS_START<br>_DATE<br><br><br> | varchar(10)<br>dd/mm/yyyy<br><br><br> | If not known leave as null. <br>For partial information use '00' where not known. E.g., if month and year are known, include '00' for day, e.g. 00/01/1988.<br><details><summary>Explanation</summary>The (best available estimate) date the participant moved into this addresss |
| 14<br><br><br><br><br><br> | <small>ADDRESS_END_DATE<br><br><br><br><br><br> | varchar(10)<br>dd/mm/yyyy<br><br><br><br><br> | Leave as null if current address <br>For partial information use '00' where not known. E.g., if month and year are known, include '00' for day, e.g. 00/01/1988. <br>Use 00/00/0000 where you do not know the date but do know it is not the current address. <br><details><summary>Explanation</summary>The (best available estimate) date the participant left this addresss |
| 15<br><br><br> | <small>DATE_OF_BIRTH<br><br><br> | varchar(10)<br>dd/mm/yyyy<br><br> | If not known leave as null <br>For partial informaton, use '01' where the day is not known. E.g., if only month and year are known, include '01' for day, e.g. 01/05/1988. |
| 16<br><br> | <small>GENDER_CD<br><br> | char(1)<br><br> | 1=male, 2=female, 7=other, 8=unspecified, 9=unknown<br><details><summary>Explanation</summary> Current gender (where recorded separately from 'sex') |
| 17<br><br> | <small>CREATE_DATE<br><br> | varchar(10)<br>dd/mm/yyyy<br> | The date on which the LPS created the file <br>Do not include 'time' |
| 18<br><br><br><br> | <small>UKLLC_STATUS<br><br><br><br> | char(1)<br><br><br><br> | An overall permission flag, which is set to 1, unless a participant should be withdrawn, where it is set to 0 to stop the future use of the participant’s data in the UK LLC TRE and to stop any flows of linked records. <br><details><summary>Explanation</summary>This indicates if a participant is considered active in UK LLC. In an LPS’s first File 1, ALL participants must be active. In subsequent iterations, the flag indicates when a participant has withdrawn consent. | 


