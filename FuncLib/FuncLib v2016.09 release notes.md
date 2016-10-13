Functions Library release v2016.09
===
<<INFO ABOUT THE RELEASE WILL GO HERE>>

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New functions
===
**REGL**
This new function clears PRISM global variables, and uses no parameters. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #299.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing functions
===
**autofill_editbox_from_MAXIS**
Added ability to read information from STAT/EMPS to the `autofill_editbox_from_MAXIS` function. This will allow scripts such as NOTES - CAF and NOTES - HRF to autofill STAT/EMPS information into the associated edit boxes in the scripts to be case noted. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #289.*

**MAXIS_dialog_navigation**
The following MAXIS navigation options have been added to the MAXIS dialog navigation function: ADME, BUDG, DFLN, DISQ, EMMA, EMPS, MMSA, PACT, PARE, REMO, SANC, SIBL, TIME, WREG and ELIG/EMER. Also removed ELIG/WB navigation as this is no longer an active program. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #287.*

**script_end_procedure**
Updated the function to allow writing to a SQL database if agencies are collecting stats, and they are using SQL vs. Access. Now, agencies with SQL databases can specify details inside their Global Variables file, and try running to a SQL table. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #295.*

**start_a_blank_case_note**
Added additional verbiage to the user message box with additional information on what to do if case notes cannot be accessed. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #240.*

**October 2016 panel changes**
Changes were made to JOBS/UNEA/SCHL panels, and the following functions have been updated to reflect this change:

* `add_JOBS_to_variable`
* `autofill_editbox_from_MAXIS`
* `write_panel_to_MAXIS_JOBS`

*Completed by Charles Potter (@CDPotter, DHS). Resolves issue #286.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Other updates
===
**Income limit constant changes**
Scripts are now prepared for the changes in income limits for SNAP gross (165%), SNAP gross/categorically (130%), and SNAP net. This also adds functionality to make this change easier each year. *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #280.*
