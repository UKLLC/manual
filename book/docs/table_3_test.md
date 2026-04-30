# DOC-DAT-044 Table 3

> Testing options


| Field<br>Order | Field<br>Name | Data<br>Type | Description<br>& values | Explanation | 
|---:|---|---|---|---|
| 1 | STUDY_ID | varchar(50) | <details><summary>STUDY_ID</summary>* Unique per participant<br>* Relate to the same person when used in File 2<br>* Same for each row of data for each individual<br>* Same for each individual across subsequent File 1s</details> | Unique LPS-generated identifier<br>(also to feature in 'File 2' attribute data file). |
| 2 | ROW_STATUS | Char(1) | <details><summary>ROW_STATUS</summary>C = Current<br>H = Historical/Alternative | Indicates whether the row of information per participant<br>is the ‘current’ row of information or a row containing<br>historical or alternative values. |
| 3 | NHS_NUMBER | varchar(10) | <details><summary>NHS_NUMBER</summary>* Preferrably new NHS ID format, but old NHS ID is preferred to no NHS ID<br>* Where LPS have encrypted 'Community Health Index' (CHI) number leave this null and instead populate NHS_S_Study_Number (field 22) with encrypted CHI<br>* Include each known NHS ID as a separate row of information. The NHS ID which is likely to be most accurate should be included in the 'current' row. Leave null if not known or if inclusion is not permitted by your DSA. </details> | NHS number, formatted with no spaces. This should<br>only be provided if the LPS’s DSA with NHSE permits onward<br>sharing of NHS IDs. <span style="color:red"> See Appendix B for more information. |



