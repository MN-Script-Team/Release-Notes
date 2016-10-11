Functions Library release v2016.09
===
<<INFO ABOUT THE RELEASE WILL GO HERE>>

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New functions
===
**function**
Description
* Parameter one
* Parameter two
* Parameter three

**function**
Description
* Parameter one
* Parameter two
* Parameter three
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing functions
===
**autofill_editbox_from_MAXIS**
Added ability to read information from STAT/EMPS to the `autofill_editbox_from_MAXIS` function. This will allow scripts such as NOTES - CAF and NOTES - HRF to autofill STAT/EMPS information into the associated edit boxes in the scripts to be case noted. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #289.*

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
Functions depreciated in this release
===

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Other updates
===

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
===
### Contribution statistics ([day before previous release] to [day before current release])

<table>
    <tr>
        <th>Scriptwriter Name</th>
        <th>Agency</th>
        <th>Commits (FuncLib)</th>
    </tr>
    <tr>
        <td><b>Veronica Cary</b></td>
        <td>DHS</td>
        <td>0</td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
