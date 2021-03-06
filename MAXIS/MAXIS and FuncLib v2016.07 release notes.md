About this release
===
This release is a relatively small release. Only two scripts were added (one is a new DAIL scrubber option), and a few functional updates were made.

BlueZone Scripts are automatically updated via GitHub, without requiring any changes to files installed locally for counties and agencies. If you appear to be missing some of these updates, consider re-installing your scripts. Contact Veronica.Cary@state.mn.us with any additional questions.

It is recommended that supervisors review these notes with staff. A PDF version of these notes is included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New scripts
===
### ACTIONS SCRIPTS
**ACCT PANEL UPDATER**
This script will either add a new ACCT panel to MAXIS or update an existing ACCT panel. It can be ran multiple times to either add/update multiple ACCT panels in any combination of add/update. It will then case note all actions upon completion of the script. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issue #2109.*

===
### DAIL SCRUBBER SCRIPTS
**POSTPONED XFS VERIFICATIONS**
This is a new DAIL Scrubber script that will case note about SNAP Closing from this DAIL Message - 'CASE AUTO-CLOSED FOR FAILURE TO PROVIDE POSTPONED VERIFICATI'. This note is specific to Expedited SNAP closing for no receipt of delayed verifications.' *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2046.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### ACTIONS SCRIPTS
**ABAWD FSET EXEMPTION CHECK**
The script will now check PBEN for any Unemployment Benefits pending as a possible ABAWD/FSET exemption. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2372.*

**PA VERIF REQUEST**
Updated script to provide full program names in addition to the program acronyms. Also added a program key for recipients to reference when the user selects to include a screen print of the issues. Updated the logic for checking for a password prompt, mandatory fields and redesigned the main dialog. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2416.*

**TYMA TIKLer**
Fixes a typo in the case note that lists 1st Quarter twice. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2384.*

===
### BULK SCRIPTS
**CASE NOTE FROM LIST**
Enhancement to the script so that it pulls wording from an existing case note if the script is started from the case note. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2395.*

**INAC SCRUBBER**
Script will now correctly loop through case number rather than getting stuck on last case number case/noted on. Also, when running the script in developer mode the script will now pause and display the case number, and the CLS number it is being transferred to. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issues #2389 and #2392.*

**REPT-GRMR LIST**
Removed default date of current month - 1 from the BULK list, enabling users to search other months besides current month - 1. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2405.*

**REPT-MAMS LIST**
Removed default date of current month - 1 from the BULK list, enabling users to search other months besides current month - 1. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2405.*

**REPT-MONT LIST**
Removed default date of current month - 1 from the BULK list, enabling users to search other months besides current month - 1. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2405.*

**REPT-MRSR LIST**
Removed default date of current month - 1 from the BULK list, enabling users to search other months besides current month - 1. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2405.*

**REPT-REVS LIST**
Due to the removal of the WB program field on the REPT screen, the location of the cash field moved. Also added enhanced password prompt, and required that users select at least one program prior to creating the Excel spreadsheet. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2409.*

**REPT-REVW LIST**
Due to the removal of the WB program field on the REPT screen, the location of the cash field moved. Also added enhanced password prompt, and required that users select at least one program prior to creating the Excel spreadsheet. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2409.*

===
### NOTES SCRIPTS
**APPROVED PROGRAMS**
Removed the navigation to SPEC/WCOM after the case note has been made. The script will revert to ending in CASE/NOTE in edit mode. Also updated the script closing text to reflect that the script is not in SPEC/WCOM. Also, for Hennepin and Ramsey County users, the Excel list (created when the case is identified as banked months) has been removed. Hennepin and Ramsey County use the process detailed in the BULK - BANKED MONTHS REPORT (https://www.dhssir.cty.dhs.state.mn.us/MAXIS/blzn/Script%20Instructions%20Wiki/Banked%20Months%20Report.aspx). For all other users that gather statistics using a database (St. Louis County) a message box will pop up informing users that the Excel spreadsheet functionality will be retired as of the August 2016 script release (08/22/16) unless there is objection by county users. Users can comment on GitHub, or email a DHS scriptwriter, if they want to see this continue. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issues #2415 and #2373.*

**BURIAL ASSETS**
A few updates to this script, which now has better functionality regarding calculation for specific assets:
* A dynamic calculator that displays current totals for counted assets and assets applied to the BFE. When the user hits a button the calculator will refresh, it will also make sure the user doesn't enter more than $1500 into the BFE and appropriately relabel the last item to push the BFE over $1500 to BFE/counted (it will also let the user know of this change and inform them to review it). This is more in line with examples found in LTC training case notes.
* A preview messagebox has been added after the user enters all of the information. This box will display the totals, what items were selected, what their items values are, and what the status of the item is (counted excluded etc). User can then go back to change things, quit, or go to case note.
* For scriptwriters: some old outdated functions were cleaned up, pulling 3 out of the functions library, and case noting procedures cleaned up as well.

*Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2343.*

**CLIENT CONTACT**
Added field for MNSURE/IC number to the dialog. This will be added to case note if used. *Completed by Kenny Lee (@kennyasalee, Ramsey County). Resolves issue #2379.*

**CLOSED PROGRAMS**
Generalized HC reinstate information on dialog to refer workers to check with policy. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2400.*

**DENIED PROGRAMS**
End message verbiage will now correctly state if a TIKL was created. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2374.*

Also, a new feature was added which finds the information for self-declaration of over-income policy on SNAP applications, and then adds the specific info to case note. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issue #2388.*

**MFIP SANCTION AND DWP DISQUALIFICATION**
Added the option to choose Dual Sanctions (CS & ES) type. Also changed sanction reason dropdown box to a combo box so the worker is able to type in a reason since dual sanctions will need to indicate two reasons. *Completed by Mel Fox (@MelissaFox-Stearns, Stearns County). Resolves issue #2418.*

===
### NOTICES SCRIPTS
**METHOD B WCOM**
Script will no longer write the health insurance premium twice on the WCOM, it will also only autofill the Medicare premium if it is coded as Y for apply to spenddown/budget on MEDI. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2433.*

**POSTPONED WREG VERIFS**
Fixes an error in determining dates used in the script. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2393.*

===
### UTILITIES SCRIPTS
**TRAINING CASE CREATOR**
Enhancing the training case generator to better create content on PBEN. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves FuncLib issue #264.*

Also, the year of birth for a client in a scenario will now be calculated by having the scenario indicate the clients age at application. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2396.*

===
### ALL SCRIPT UPDATES
**ABAWD months in case notes**
 If client hasn't used 2nd set of ABAWD months, the 2nd set number will register no months, and the verbiage about the second set months used will not be added to the edit box. Also, if client is a mandatory FSET participant (with an ABAWD counted month) and has not used any ABAWD months, the verbiage about the list of used months will not be added to the edit box. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #262.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Functions Library (FuncLib) updates (for scriptwriters)
===
### Updated functions
**script_end_procedure**
For stats-collecting agencies, the database connection will now explicitly close prior to exiting. End users should not notice any differences. Also, a "pass through" function was installed for scriptwriters. To create a message on the Access database without creating a corresponding pop-up, simply use `script_end_procedure("~PT: [message goes here]")`. The contents of the message will be passed through to the database without showing up as a pop-up. *Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issues #217 and #257.*

**write_panel_to_MAXIS_ACCT**
Updating `write_panel_to_MAXIS_ACCT` to account for moving Account Balance Verification field. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves FuncLib issue #245.*

**worker_signature**
The `worker_signature` determination was moved from Global Variables to FuncLib. *Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issue #254.*

**OTHER FUNCTIONS**
Removed 3 functions that were only being used in the NOTES - BURIAL ASSETS script and didn't have any other functionality outside of that script: `new_BS_BSI_heading`, `new_CAI_heading`, and `new_service_heading`. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves FuncLib issue #247.*

===
### Depreciated and removed functions for this release
* memb_navigation_next
* memb_navigation_prev
* navigation_buttons
* panel_navigation_next
* panel_navigaton_prev
* stat_navigation
* script_end_procedure_wsh
* step_through_handling
* sort_numeric_array_ascending (removed completely)
* sort_numeric_array_descending (removed completely)

*Script depreciation completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #252.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
===
### Contribution statistics (06/26/2016 to 07/24/2016)

<table>
    <tr>
        <th>Scriptwriter Name</th>
        <th>Agency</th>
        <th>Commits (Scripts)</th>
        <th>Commits (FuncLib)</th>
        <th>Commits (Total)</th>
    </tr>
    <tr>
        <td>Ilse Ferris</td>
        <td>Hennepin County</td>
        <td>14</td>
        <td>15</td>
        <td><b>29</b></td>
    </tr>
    <tr>
        <td>Casey Love</td>
        <td>Ramsey County</td>
        <td>14</td>
        <td>0</td>
        <td><b>14</b></td>
    </tr>
    
    <tr>
        <td>Veronica Cary</td>
        <td>DHS</td>
        <td>8</td>
        <td>3</td>
        <td><b>11</b></td>
    </tr>
    <tr>
        <td>Charles Potter</td>
        <td>Anoka County</td>
        <td>7</td>
        <td>2</td>
        <td><b>9</b></td>
    </tr>
    <tr>
        <td>Tim Delong</td>
        <td>Stearns County</td>
        <td>4</td>
        <td>0</td>
        <td><b>4</b></td>
    </tr>
    <tr>
        <td>Kenny Lee</td>
        <td>Ramsey County</td>
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
    <tr>
        <td>Robert Fewins-Kalb</td>
        <td>Anoka County</td>
        <td>0</td>
        <td>1</td>
        <td><b>1</b></td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
