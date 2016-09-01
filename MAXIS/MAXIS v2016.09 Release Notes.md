About this release
===
<<INFO ABOUT THE RELEASE WILL GO HERE>>

BlueZone Scripts are automatically updated via GitHub, without requiring any changes to files installed locally for counties and agencies. If you appear to be missing some of these updates, consider re-installing your scripts. Contact Charles.Potter@state.mn.us with any additional questions.

It is recommended that supervisors review these notes with staff. A PDF version of these notes is included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New scripts
===
### CATEGORY
**SCRIPT**
Text

**SCRIPT**
Text

===
### CATEGORY
**SCRIPT**
Text

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### ACTIONS
**ACCT UPDATER**
Script will now warn users if unable to edit, it can update if there are more than 9 account panels. Also implemented some behind the scenes revamping including:
- deleted extraneous dialog
- script will now convert what it finds on ACCT panel for all variables on the dialog
- new handling no longer requiring to enter count codes for programs that aren't active/pending
*Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2465.*

**FSET SANCTION**
Option added within the 'resolved sanction' option: If the recipient resolves their sanction prior to the sanction effective/imposed date, the case note reflects that the sanction was deleted, and the 'number of sanctions' field is cleared on STAT/WREG. The script has also moved from the MAIN ACTIONS menu to the ABAWD ACTIONS menu, and several functions and mandatory field criteria was updated on the back end. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2480.*

### BULK
**BANKED MONTHS REPORT**
Several enhancements to the script have been made. ABAWD month counting and filtering of banked months has been streamlined. All other updates are to add rejected cases to the rejected banked months list, along with the reason for rejection. Cases are now rejected for the following reasons:
- Cases that can't access person notes
- Cases that are coded 30/11
- Cases that aren't coded as a 30/10
- Cases that are prorated, but the approval is not prorated
- Cases where the script cannot access the ABAWD tracking record
- Cases where the report date is not coded as a counted ABAWD month on the ABAWD tracking record
*Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2479.*

**CASE TRANSFER**
A limiter has been added so that the script run time will be reduced if only a small number of cases need to be found. *Completed by Casey Love (@C-Love, Ramsey County). Resolved issue #2492.*

### NAV
**DAIL/WRIT**
Script has been reworked so it no longer transmits off of the current panel/list allowing user to keep the case numbers they want to see in front of them to enter in the script if needed. *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2475.*

### NOTES
**ABAWD FSET EXEMPTION CHECK**
Added gender dropdown list and mother/member number drop down list for baby born portion *Completed by Kenny Lee (@Kennyasalee, Ramsey County). Resolves issue #2450 & 2451.*

**EXPEDITED SCREENING**
Script is now prepared for changes to shelter deduction standards effective 10/1/16 *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2464.*

**MAIN MENU**
removed outdated 'new' script indicators from the NOTES - MAIN MENU *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2474.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Scripts retired in this release
===

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Other updates
===

**10/16 Panel Changes**
Scripts were updated to take into account the changes for 10/16 to JOBS/UNEA/SCHL Critical changes were made a priorty while none critical changes are being tackles as they arise. *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2485.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
===
### Contribution statistics (8/22/16 to 9/25/16)

<table>
    <tr>
        <th>Scriptwriter Name</th>
        <th>Agency</th>
        <th>Commits (MAXIS)</th>
    </tr>
    <tr>
        <td><b>Casey Love</b></td>
        <td>Ramsey</td>
        <td>2</td>
    </tr>
    <tr>
        <td><b>Charles Potter</b></td>
        <td>DHS</td>
        <td>11</td>
    </tr>
    <tr>
        <td><b>Ilse Ferris</b></td>
        <td>Hennepin</td>
        <td>19</td>
    </tr>
    <tr>
        <td><b>Kenny Lee</b></td>
        <td>Ramsey</td>
        <td>3</td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
