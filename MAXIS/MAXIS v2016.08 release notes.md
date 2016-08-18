About this release
===
Smaller release this month due to the change of hands. 

BlueZone Scripts are automatically updated via GitHub, without requiring any changes to files installed locally for counties and agencies. If you appear to be missing some of these updates, consider re-installing your scripts. Contact Charles.Potter@state.mn.us with any additional questions.

It is recommended that supervisors review these notes with staff. A PDF version of these notes is included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### ACTIONS SCRIPTS
**ABAWD FSET EXEMPTION CHECK**
Fixed a bug for cases in which HH member has more than one job. The 1st job was being skipped. All jobs now being read, and included in income calculation. 
Also fixed a bug to correctly multiply prospective hours for all jobs. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2456.*

**ABAWD BANKED MONTHS FIATER**
Updated the script to account for cases that have the initial month coded as an "X" on the ABAWD tracking record. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2454.*

**TRANSER CASE**
Script will now correctly find the new worker's name (it was only reading for Aliases before) and include the new workers complete information in the body of the MEMO. *Completed by Charles Potter (@cdpotter, DHS). Resolves issue #2438.*

### BULK SCRIPTS
**BANKED MONTH REPORT**
Fixed a bug for cases in which HH member has more than one job. The 1st job was being skipped. All jobs now being read, and included in income calculation. 
Also fixed a bug to correctly multiply prospective hours for all jobs. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2456.*

**REPT PND2**
For MULTICOUNTY users this script was using the wrong variable to determine the list of users to run on. *Completed by Charles Potter (@cdpotter, DHS). Resolves issue #2458.*

### DAIL SCRUBBER SCRIPTS
**ABAWD FSET EXEMPTION CHECK**
Fixed a bug for cases in which HH member has more than one job. The 1st job was being skipped. All jobs now being read, and included in income calculation. 
Also fixed a bug to correctly multiply prospective hours for all jobs. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2456.*

### NOTES SCRIPTS
***APPROVED PROGRAMS***
Interest was presented in keeping the excel functionality available for the banked months tracking. As such it won't be retired and the warning message box has been removed. *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2373.*

**CSR**
Added GRH checkbox for users to select CSR, added ELIG/GRH navigation button to dialogs. Also updated date variables to global constants and footer month functions on the back end. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2453.*

**LTC - TRANSFER PENALTY**
Name of script had incorrect category name. Changed category name from NOTE to NOTES. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2441.*

**OVERPAYMENT**
Added a new dropdown to select if the claim can be collected (options are YES, NO, or N/A), and added a field for workers to enter calculations and explanations as to why or why not the claim is collectible. *Completed by Charles Potter (@cdpotter, DHS). Resolves issue #2452.*

### UTILITIES SCRIPTS
**INFO**
Updating contact information for Charles and Veronica. *Completed by Charles Potter (@cdpotter, DHS). Resolves issue #2444.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Scripts retired in this release
===
### BULK SCRIPTS
**MAGI/NON-MAGI REPORT**
Per MNIT they do not want counties using this script to identify who is migrating. As such we have been asked to remove the script. *Completed by Charles Potter (@cdpotter, DHS). Resolves issue #2447.*

===

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
===
### Contribution statistics (07/25/2016 to 08/22/16)

<table>
    <tr>
        <th>Scriptwriter Name</th>
        <th>Agency</th>
        <th>Commits (MAXIS)</th>
        <th>Commits (FuncLib)</th>
        <th>Commits (Total)</th>
    </tr>
    <tr>
        <td>Ilse Ferris</td>
        <td>Hennepin County</td>
        <td>12</td>
        <td>1</td>
        <td><b>13</b></td>
    </tr>
        <tr>
        <td>Charles Potter</td>
        <td>DHS</td>
        <td>5</td>
        <td>0</td>
        <td><b>5</b></td>
    </tr>
</table>

