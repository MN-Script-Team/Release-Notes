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
**ABAWD BANKED MONTHS FIATER**
Adding new income types for actions scripts. New income types include:
JOBS: T Training Program P Service Program R Rehab Program
UNEA: 47 Counted Tribal Income 48 Trust Income 49 Non-Recurring Income > $60 per Quarter *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2496.*

**ACCT UPDATER**
Script will now warn users if unable to edit, it can update if there are more than 9 account panels. Also implemented some behind the scenes revamping including:
- deleted extraneous dialog
- script will now convert what it finds on ACCT panel for all variables on the dialog
- new handling no longer requiring to enter count codes for programs that aren't active/pending
*Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2465.*

**FSET SANCTION**
Option added within the 'resolved sanction' option: If the recipient resolves their sanction prior to the sanction effective/imposed date, the case note reflects that the sanction was deleted, and the 'number of sanctions' field is cleared on STAT/WREG. The script has also moved from the MAIN ACTIONS menu to the ABAWD ACTIONS menu, and several functions and mandatory field criteria was updated on the back end. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2480.*

**LTC SPOUSAL ALLOCATION FIATER**
Adding new income types for actions scripts. New income types include:
JOBS: T Training Program P Service Program R Rehab Program
UNEA: 47 Counted Tribal Income 48 Trust Income 49 Non-Recurring Income > $60 per Quarter *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2496.*

**NEW JOB REPORTED**
Adding new income types for actions scripts. New income types include:
JOBS: T Training Program P Service Program R Rehab Program
UNEA: 47 Counted Tribal Income 48 Trust Income 49 Non-Recurring Income > $60 per Quarter *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2496.*

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

**MAIN MENUS**
added third BULK Main Menu category, and renamed one of the existing categories. New categories are: BULK ACTIONS (previously BULK), ENHANCED LISTS (lists that contain logic, but not actions) and BULK LISTS (the name of this category did not change, but some of the scripts were moved to the ENHANCED LISTS category). *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2514.*

**REVW/MONT CLOSURES**
Updated HC reinstatement and new intake date to reflect the 4 month reinstatement period for all HC programs (not MAGI only). *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2503.*

### DAIL SCRUBBER
**CITIZENSHIP VERIFIED**
added option for user to navigate back to the dail. *Completed by Charles Clark (@Senhorc, Hennepin County). Resolved issue #2470.*

**CSES DAIL SCRUBBER**
Script will branch into two scripts for a bit while testing commences. New script will:

Gathers DAIL messages and creates a spreadsheet to display and work with them
Identify which UNEA panel each message is associated with
Determines if SNAP or MFIP case and if HRF or REVW is due
If SNAP active the case will look at SNAP ELIG to gather budget information
If SNAP active, UNEA detail will be added to a new worksheet on Excel document
Dialog will appear based on programs active. Workers will be able to add notes, sign case note, indicate if Excel sheet should remain open at end of script, and indicate if additional review is needed. IF SNAP is active and there is either a change in the amount of CS OR the income appears to exceed 130% FPG, the script will default to having the panels reviewed by worker.
If SNAP case needs income reviewed, a dialog for each UNEA panel will ask worker if income needs adjusting (Yes/No only).
IF MFIP, script will add worksheet to Excel document and then attempt to update UNEA upon worker confirmation.
Case note! and close spreadsheet
*Completed by Casey Love (@C-love, Ramsey County) and Veronica Cary (@theVKC DHS). Resolved Issue #1714.*

The script is now case noting correctly after reviewing UNEA panels. Added logic to check if it made it to note, and fixed typos in case note function call. *Completed by David Courtright (St Lluis County) Resolved Issue #2500.*

### NAV
**DAIL/WRIT**
Script has been reworked so it no longer transmits off of the current panel/list allowing user to keep the case numbers they want to see in front of them to enter in the script if needed. *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2475.*

### NOTES
**ABAWD FSET EXEMPTION CHECK**
Added gender dropdown list and mother/member number drop down list for baby born portion *Completed by Kenny Lee (@Kennyasalee, Ramsey County). Resolves issue #2450 & 2451.*

**CAF**
Added EMPS panel field to the CAF 1 dialog. This field will be auto-filled with the information for all HH members on the case. Also added EMPS, SANC and TIME navigation buttons, removed the WB ELIG navigation and updated the password check handling on the back end. 
For Hennepin County and Ramsey County workers: a checkbox has been added "Sent MFIP financial orientation DVD to participant(s)." This check box will case note if a participant has been given a financial orientation DVD." *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2487.*

**COMBINED ANNUAL RENEWAL**
The script has been updated to show what programs are being recertified in the case note. *Completed by Mel Fox (@MelissaFox-Stearns Stearns County). Resolved issue #2512*

**ES REFERRAL**
Option to schedule or reschedule an ES appt, and added a field for vendor numbers in the dialog which will also appear in the case note. Also added handling for checking for users who have passworded out, and allows them to enter password and continue. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2504.*

**EXPEDITED SCREENING**
Script is now prepared for changes to shelter deduction standards effective 10/1/16 *Completed by Charles Potter (@CDPotter, DHS). Resolves issue #2464.*

**FOSTER CARE HCAPP** 
Added fields for HHcomp and assets *Completed by Roy Walz (@RoyStearns, Stearns). Resolved issue #2509**

***HCAPP***
Added a Combo-box to choose the type of HCAPP that was received. *Completed by Roy Walz (@RoyStearns, Stearns). Resolved issue #2495**

**HRF**
Added EMPS panel field to the main dialog. This field will be auto-filled with the information for all HH members on the case. Also added EMPS, SANC and TIME navigation buttons, update dates to global constants and updated the password check handling on the back end. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2498.*

**MAIN MENU**
removed outdated 'new' script indicators from the NOTES - MAIN MENU *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2474.*

removed NOTES - MFIP SANCTION CURED as it is now incorporated into NOTES - MFIP SANCTION/DWP DISQUALIFICATION *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2506.*

**MFIP SANCTION/DWP DISQUALIFICATION**
Merged NOTES - MFIP SANCTION CURED into NOTES - MFIP SANCTION/DWP DISQUALIFICATION. Users will now select the action type (applying the sanction/disq. or cure sanction/disq.), then will be directed to the option selected. 

The following options have been added to the 'applying the sanction/disq.' option: pre/post 60 selection option, pre/post 60 notes field to discuss pre/post 60 information and changed "no show to orientation" to "Failed to attend orientation" in the "type of sanction" droplist.

The following options have been added to the 'cure sanction/disq' option: member number field, financial orientation information and good cause information fields; TIME, SANC and EMPS navigation buttons, and an option to TIKL for 6 months to evaluate mandatory vendor removal (if applicable). The TIKL will be created for the 1st day of the month of the 6th month (example TIKL created on 09/08/2016. TIKL will appear on: 03/01/2017. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2506 & 2507.*

**MTAF**
for Hennepin and Ramsey county users- added checkbox to case note that the MFIP financial orientation DVD has been sent (if checked). Also removed outdated password functionality. This was previously replaced with updated password functionality. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2505.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Scripts retired in this release
===

**NOTES - MFIP SANCTION CURED**
MFIP SANCTION CURED has been retired as it is now incorporated into NOTES - MFIP SANCTION/DWP DISQUALIFICATION.  *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolved issue #2506.*

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
        <td>5</td>
    </tr>
    <tr>
        <td><b>Charles Clark</b></td>
        <td>Hennepin</td>
        <td>2</td>
    </tr>
    <tr>
        <td><b>Charles Potter</b></td>
        <td>DHS</td>
        <td>14</td>
    </tr>
   <tr>
        <td><b>David Courtright</b></td>
        <td>St Louis</td>
        <td>1</td>
    </tr>
    <tr>
        <td><b>Ilse Ferris</b></td>
        <td>Hennepin</td>
        <td>35</td>
    </tr>
    <tr>
        <td><b>Kenny Lee</b></td>
        <td>Ramsey</td>
        <td>3</td>
    </tr>
    <tr>
        <td><b>Mel Fox</b></td>
        <td>Stearns</td>
        <td>2</td>
    </tr>
    <tr>
        <td><b>Roy Walz</b></td>
        <td>Stearns</td>
        <td>3</td>
    </tr>
        <tr>
        <td><b>Veronica Cary</b></td>
        <td>DHS</td>
        <td>19</td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
