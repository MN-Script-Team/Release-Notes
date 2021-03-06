About this release
===
The June 2016 release of BlueZone Scripts includes several new bulk list generator scripts, as well as a very powerful new scrubber: the "REVS Scrubber". This new script will create a list of cases that need a SNAP (or cash) interview from REPT/REVS, designate a time for the interview, and send an appointment letter en masse to all affected cases before a CAF has been turned in (improving CAF return rates and reducing cutoff notices). This release also cuts off the old menus for alpha-split NOTES and the MEMOS button on Power Pads. Agencies will need to update in order to regain access to these scripts. 

BlueZone Scripts are automatically updated via GitHub, without requiring any changes to files installed locally for counties and agencies. If you appear to be missing some of these updates, consider re-installing your scripts. Contact Veronica.Cary@state.mn.us with any additional questions.

It is recommended that supervisors review these notes with staff. A PDF version of these notes is included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New scripts
===
### BULK SCRIPTS
**MAGI/NON-MAGI REPORT**
This new script checks the inputted MAXIS caseloads for MAGI/Non-MAGI Health Care cases. Users have the option of adding the caseload's supervisor to the output. Additionally, users have the option of adding the status of CASH and SNAP on the MAXIS case. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #2112.*

**REVS SCRUBBER**
Creates a list of cases from REPT/REVS that need a SNAP (or cash) interview, and schedules the interview, sends the appointment letter, case notes and TIKL's the interview information for a caseload (or multiple caseloads). *Completed by Veronica Cary (@theVKC, DHS), David Courtright (@courtrightd, St. Louis County), Ilse Ferris (@IlseFerris, Hennepin County), Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County), Casey Love (@C-Love, Ramsey County), and Charles Potter (@CDPotter, Anoka County). Resolves issue #710.*

**REPT-GRMR LIST**
Bulk script that creates a list of cases in REPT/MAMS on an Excel spreadsheet. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2319.*

**REPT-IEVC LIST**
This is a new script that will create a report of information found on IEVC, including statistics and overdue instances. This script can also be run for the entire agency. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2281.*

**REPT-MAMS LIST**
Bulk script that creates a list of cases in REPT/MAMS on an Excel spreadsheet. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2318.*

**REPT-MONT LIST**
Bulk script that creates a list of cases in REPT/MONT on an Excel spreadsheet. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2278.*

**REPT-MRSR LIST**
Bulk script that creates a list of cases in REPT/MRSR on an Excel spreadsheet. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2279.*

===
### UTILITIES SCRIPTS
**COPY CASE NOTE ELSEWHERE**
This script will allow users to copy a case note into claim notes or into a MEMO. NOTE: MEMO has a smaller space for writing so not all case notes will fit. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2263.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### ACTIONS SCRIPTS
**ABAWD FSET EXEMPTION CHECK**
Reworking verbiage to better follow policy (Combined Manual citation: 0028.06.12). It will now read: "appears to be working 30 hours/wk (regardless of wage level) or earning equivalent of 30 hours/wk at federal minimum wage. Please review for ABAWD and SNAP E&T exemptions." rather than not mentioning working 30 hours a week. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2270.*

**CHECK EDRS**
Additional safeguards have been installed which should prevent users from being passworded out. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2339.*

**COPY PANELS TO WORD**
This script has been changed to a UTILITIES script instead of an ACTIONS script. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2290.*

**HOUSING GRANT MONY CHCK ISSUANCE**
This script name was too long. Renamed the script to **ACTIONS - HG SUPPLEMENT**. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2291.*

**TRANSFER CASE**
Updated to notify worker if SPEC/MEMO is unable to be accessed. Added verbiage to include this could be because the worker does not have authorization to send a SPEC/MEMO. Script originally only had a message that the worker could be in inquiry mode. *Completed by Mel Fox (@MelissaFox-Stearns, Stearns County). Resolves issue #2269.*

**MAIN MENU**
The Utilities menu button has been removed from the Actions main menu, as it is now on its own button on the Power Pad. Also, an incorrect reference to Notices scripts was replaced. Finally, a new layout (which integrates SIR instructions) has been deployed. *Completed by Veronica Cary (@theVKC, DHS). Resolves issues #2288 and #2268.*

===
### BULK SCRIPTS
**CASE TRANSFER**
Fixed the script so that the cases will transfer without a MAXIS error. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2246.*

**CHECK SNAP FOR GA RCA**
Fixed a bug that was causing holes in the output of the report. Not all cases were selected, and this has been resolved. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #2364.*

**DAIL REPORT**
Fixes a bug so the script does not get stuck if a worker has no DAILs listed. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2309.*

**INAC SCRUBBER**
The INAC Scrubber can now be used while bypassing MMIS (should the user not have access). In these cases, as a safeguard, it will not transfer cases that closed in the INAC month on health care to Closed Cases. Additionally, err_msg handling has been added for simpler data validation, and the dialog has been renamed Dialog1 for chainloading. Finally, the global variable for providing a 4 month health care reinstate period has been removed, all cases will now follow that logic. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issues #2292 and #2336.*

**REPT-ARST LIST**
Enhancement to the script that will include the total case counts for workers to the report, since these are different from the program based counts. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2131.*

**REPT-PND1 LIST**
A variable has been updated to look for an entire case number rather than one digit, eliminating missed cases on this bulk list. *Completed by Travis Farleigh (@Farleight, Carlton County). Resolves issue #2258.*

**REPT-REVS LIST**
A variable has been updated to look for an entire case number rather than one digit, eliminating missed cases on this bulk list. *Completed by Travis Farleigh (@Farleight, Carlton County). Resolves issue #2258.*

**REPT-REVW LIST**
A variable has been updated to look for an entire case number rather than one digit, eliminating missed cases on this bulk list. *Completed by Travis Farleigh (@Farleight, Carlton County). Resolves issue #2258.*

**REVW/MONT CLOSURES**
Script will now correctly case note MAGI reinstate dates. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2265.*

**TARGETED SNAP REVIEW SELECTION**
The script will now only select active cases that have had a SNAP approval in current month minus one, to align with review month for CAPER cases. Also, corrected an error that was preventing the script from selecting cases for the audit spreadsheet in certain circumstances. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issues #2262 and #2325.*

===
### DAIL SCRUBBER SCRIPTS
**ABAWD FSET EXEMPTION CHECK**
Reworking verbiage to better follow policy (Combined Manual citation: 0028.06.12). It will now read: "appears to be working 30 hours/wk (regardless of wage level) or earning equivalent of 30 hours/wk at federal minimum wage. Please review for ABAWD and SNAP E&T exemptions." rather than not mentioning working 30 hours a week. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2270.*

**Send NOMI**
Removed option for user to select whether or not renewal forms were received in the agency or not per policy clarification (TE02.05.15). *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2347.*

===
### NAV SCRIPTS
**PRISM SCREEN FINDER**
Updating statistics code so that agencies that collect usage statistics calculate accurate information. *Completed by Wendy LeVesseur (@levesswe, Anoka County). Resolves issue #2217.*

===
### NOTES SCRIPTS
**APPLICATION RECEIVED**
A bug was fixed in the functions library that was causing a single digit for MAXIS footer month (causing the script to enter the footer month into the wrong space in the footer month field), it will now correctly enter the two digit standard for scripts for the MAXIS footer month. *Completed by Casey Love (@C-Love, Ramsey County). Resolves FuncLib issue #232.*

**APPROVED PROGRAMS**
A warning message has been added to pop up when this script is run on an MFIP or DWP case that has a child under 12 months listed on it. These cases require a workaround and are often coded incorrectly. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2361.*

**BURIAL ASSETS**
You can now list specific items and/or services as being applied to the BFE. This will then be calculated and displayed in detail on the case note. Also added alternative container to Burial space/items list. Added luncheon, and medical exam fee to cash advance items. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2245.*

**CLOSED PROGRAMS**
Sanction period will now contact days as opposed to only month/year giving a better indicator of the actual period of the sanction. Also, the script will now correctly handle expedited snap closures for no postponed verification returned. Per CM 4.12; 5.09.06; 5.12.15.09; 05.12.15.03; 05.12.15.15 clients who apply on or before the 15th of a month have 30 days from application date to turn in verification. After that they must reapply. Clients who apply after the 15th have until the date of closure to turn in verification. After that they must reapply. Also, changed HCPM button to direct to new HC Eligibility program manual. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issues #2264, #2333, and #2334.*

**LTC - ASSET ASSESSMENT**
The `EMReadScreen` function was accidentally written as `EMReadScreacen` when reading marital assets, causing an impassable error. Corrected the spelling of the function. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2285.*

**LTC - COLA SUMMARY 2016**
The script can now enter the month the worker chooses, rather than being limited to one approval month per COLA cycle. The name of this script has been changed to **LTC - COLA SUMMARY** as a result. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2276.*

===
### NOTICES SCRIPTS
**METHOD B WCOM**
Removed duplicate wording and minor spelling error. *Completed by Katie Martini (@KateiMartini, Washington County) and Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2230.*

**SNAP E&T LETTER**
Removed verbiage for all users: "A verification request for proof of contact with E & T within 30 days will also need to be sent to the recipient". It has been clarified from Karen Nelson-Huss, DHS, that a verification request does not need to be sent in this instance. Also added Somali-language E & T orientation for Hennepin County users. This orientation begins on 07/12/16, and users can start scheduling clients for this orientation on 07/06/16. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2356.*

===
### UTILITIES SCRIPTS
**INFO**
A new scriptwriter from Ramsey County (Kenny Lee) has been added to the scriptwriter list. *Completed by Kenny Lee (@kennyasalee, Ramsey County). Resolves issue #2304.*

**TRAINING CASE CREATOR**
The Training Case Creator will now pend cases up to current month -11 so that ER processing can be trained. There is also an option to set the HC Review dates both to be 12 months from the date of application. Additionally if a scenario includes an undocumented person, no SSN will be created. The scenario spreadsheet has been updated to accommodate these changes. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2304.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Scripts retired in this release
===
### OTHER SCRIPTS
**MAIN MENU SCRIPTS**
The old alpha-split based NOTES main menu scripts, as well as the old MEMOS main menu scripts, have been deleted as they are now depreciated. Agencies are expected to have updated their Power Pads to the latest revision. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2194.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Functions Library (FuncLib) updates (for scriptwriters)
===
### New functions
**create_array_of_all_active_x_numbers_by_supervisor**
This new function can be used for generated caseload stats requesting data for X numbers according to their supervisor. The function can accept a list of supervisor X numbers separated by comma. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves FuncLib issue #243.*

**declare_main_menu_dialog**
This new function generates a dynamic main menu based on the `COMPLETE LIST OF SCRIPTS.vbs` file in the main GitHub repository. *Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issue #163.*

**month_change**
This is a new function that generates a month/year that is a given interval added or subtracted from an original month/year. *Completed by Casey Love (@C-Love, Ramsey County). Resolves FuncLib issue #194.*

===
### Updated functions
**convert_date_into_MAXIS_footer_month**
A bug was fixed that was causing a single digit for MAXIS footer month (causing the script to enter the footer month into the wrong space in the footer month field), it will now correctly enter the two digit standard for scripts for the MAXIS footer month. *Completed by Casey Love (@C-Love, Ramsey County). Resolves FuncLib issue #232.*

**MAXIS_footer_finder**
This function now has the ability to correctly pull the footer month/year information off of SPEC/MEMO screens. Prior to this it was occasionally breaking. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves FuncLib issue #225.*

===
### Depreciated functions
Many outdated functions have been completely removed from the Functions Library. The following functions no longer work:

* `ERRR_screen_check`is now depreciated, its functions incorporated into other navigation scripts.
* `MAXIS_check_function` is now `check_for_MAXIS`
* `navigate_to_screen` is now `navigate_to_MAXIS_screen`
* `write_editbox_in_case_note` is now `write_bullet_and_variable_in_case_note`
* `write_new_line_in_case_note` is now `write_variable_in_case_note`
* `write_new_line_in_spec_memo` is now `write_variable_in_spec_memo`
* `worker_county_code_determination` is now `get_county_code`
* `write_TIKL_function` is now `write_variable_in_TIKL`

*Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issue #219.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Other updates
===
### Excel files for scripts
**Banked Month Report Files**
Excel files have been added to GitHub for download. These files are formatted and set up for use with the BULK - Banked Months Report. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2306.*

**New folder**
All Excel files have been moved to their own folder on the GitHub project page. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2313.*

### README.md
**When to remove a script**
The README was updated to include guidelines about when scripts should be removed from the project. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2344.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
===
### Contribution statistics (05/22/2016 to 06/26/2016)

<table>
    <tr>
        <th>Scriptwriter Name</th>
        <th>Agency</th>
        <th>Commits (Scripts)</th>
        <th>Commits (FuncLib)</th>
        <th>Commits (Total)</th>
    </tr>
    <tr>
        <td>Veronica Cary</td>
        <td>DHS</td>
        <td>35</td>
        <td>8</td>
        <td><b>43</b></td>
    </tr>
    <tr>
        <td>Casey Love</td>
        <td>Ramsey County</td>
        <td>40</td>
        <td>2</td>
        <td><b>42</b></td>
    </tr>
    <tr>
        <td>Ilse Ferris</td>
        <td>Hennepin County</td>
        <td>42</td>
        <td>0</td>
        <td><b>42</b></td>
    </tr>
    <tr>
        <td>Charles Potter</td>
        <td>Anoka County</td>
        <td>22</td>
        <td>3</td>
        <td><b>25</b></td>
    </tr>
    <tr>
        <td>Robert Fewins-Kalb</td>
        <td>Anoka County</td>
        <td>7</td>
        <td>1</td>
        <td><b>8</b></td>
    </tr>
    <tr>
        <td>Travis Farleigh</td>
        <td>Carlton County</td>
        <td>3</td>
        <td>0</td>
        <td><b>3</b></td>
    </tr>
    <tr>
        <td>David Courtright</td>
        <td>St. Louis County</td>
        <td>2</td>
        <td>0</td>
        <td><b>2</b></td>
    </tr>
    <tr>
        <td>Kenny Lee*</td>
        <td>Ramsey County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
    <tr>
        <td>Wendy LeVesseur</td>
        <td>Anoka County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
    <tr>
        <td>Melissa Fox</td>
        <td>Stearns County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
