About this release
===
This release of BlueZone Scripts is a small release which includes a few new helpful tools, including a neat new PRISM Screen Finder for MAXIS users built by Wendy LeVesseur, a Child Support worker from Anoka County. Scriptwriters statewide spent much of this release cycle working on major projects expected in the next few months, including new workflow scripts and updates to popular scripts such as CAF and the DAIL Scrubber.

BlueZone Scripts are automatically updated via GitHub, without requiring any changes to files installed locally for counties and agencies. If you appear to be missing some of these updates, consider re-installing your scripts. Contact Veronica.Cary@state.mn.us with any additional questions.

It is recommended that supervisors review these notes with staff. A PDF version of these notes is included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New scripts
===
### ACTIONS SCRIPTS
**HOUSING GRANT MONY/CHCK ISSUANCE**
This is a new script for MFIP housing grant cases that should have been issued in prior months. This script will ensure that an issuance has not already occurred for the case and month selected, and will complete the MONY/CHCK per the instructions in the Housing grant bulletin, and will case note the action. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2081.*

===
### BULK SCRIPTS
**HOUSING GRANT EXEMPTION FINDER**
This is a new script that creates a list of the rolling 12 months of housing grant issuances for MFIP recipients who've met an exemption. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2001.*

**TARGETED SNAP REVIEW SELECTION**
This is a new script that will allow agencies to select SNAP cases for internal review based on specific criteria to help identify error-prone cases. Selects both PAR (ACTIVE) and CAPER (closed/denied) cases for review. The script collects cases off REPT/ACTV and REPT/INAC and adds those cases meeting selection criteria to a spreadsheet. Once the lists have been built, it selects at random the specified number of each review type and adds them to a new sheet to be assigned for review. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2093.*

===
### NOTES SCRIPTS
**DECEASED CLIENT SUMMARY**
Script for case noting details about a deceased client. *Completed by Ann Sunderman (@asunderman, Le Sueur County). Resolves issue #2054.*

===
### NOTICES SCRIPTS
**BANKED MONTHS WCOMS**
Adds WCOMS based on selection from 3 options:
* All banked months used
  * _"You have been receiving SNAP banked months. Your SNAP is closing for using all available banked months. If you meet one of the exemptions listed above AND all other eligibility factors you may still be eligible for SNAP. Please contact your financial worker if you have questions."_
* Banked months notifier
  * _"You have used all of your available ABAWD months. You may be eligible for SNAP banked months if you are cooperating with Employment services. Please contact your financial worker if you have questions."_
* Closing for E/T non-coop 
  * _"You have been receiving SNAP banked months. Your SNAP case is closing because CLIENT NAME did not meet requirements of working with Employment and Training. If you feel you have Good Cause for not cooperating with this requirement please contact your financial worker before your SNAP closes. If your SNAP closes for not cooperating with Employment and Training you will not be eligible for future banked months. If you meet an exemption listed about AND all other eligibility factors you may still be eligible for SNAP. Please contact your financial worker if you have questions."_
  
  *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2039.*
  
**VERIFICATIONS STILL NEEDED**
This script is meant to be used when several verifications have been received from the client but there is still outstanding information needed to determine eligibility. It will case note all outstanding information entered in to the script and then open a Word document, and list the information there as well to be sent out to the client, informing them that more information is still needed. *Completed by Laura Larson (@LaLarson, Olmsted County). Resolves issue #2060.*

===
### OTHER NAV SCRIPTS
**PRISM SCREEN FINDER**
This new script is intended to assist financial workers in navigating to popular screens in PRISM. To use, simply press the button for the screen you are looking to go to when open in PRISM. At the screen, press F1 in the case number, or MCI number field to search for and select the participant whose information you would like to see. *Completed by Wendy LeVesseur (@levesswe, Anoka County). Resolves issue #2074.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### ACTIONS SCRIPTS
**PA VERIF REQUEST**
Adds a reminder on the dialog that users should not share FTI information with other agencies by using this form. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2103.*

**PAYSTUBS RECEIVED**
An issue where the script was not returning to the proper JOBS panel was resolved. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #2065.*

**SHELTER EXPENSE VERIF RECEIVED**
A bug causing cases with room & board to behave incorrectly was resolved. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2047.*

**MAIN MENU**
Menu has been reworked behind-the-scenes to better fit the standard set by the BULK, NOTES, and NOTICES menus. Workers should be largely unaffected. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issues #1998 and #2125.*

===
### BULK SCRIPTS
**CHECK SNAP FOR GA RCA**
Script users are given the option to add the worker's supervisor to the script's output. Also, the script's output has been expanded to display the GA monthly grant and the GA issuance amount separately (should the client happen to have a GA overpayment). *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves part of issue #2061 and resolves issue #2104.*

**FIND PANEL UPDATE DATE**
Script users are given the option to add the worker's supervisor to the script's output. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves part of issue #2061.*

**UPDATE EOMC LIST**
Corrected a run-time error that prevented the script from functioning on some spreadsheets. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2077.*

===
### DAIL SCRUBBER SCRIPTS
**SEND NOMI**
Verbiage on question about when to send NOMI was reworked to read better to end users. Corrected issue that caused infinite loop when trying to run in inquiry. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2098.*

===
### NOTES SCRIPTS
**DENIED PROGRAMS**
Script will now better prompt user for information regarding withdrawn programs. It will check PND2 and based on what worker has coded try to insure worker completes dialog properly based on the types of denials. Also reworked verbiage on the 30 day reinstate checkbox to be more clear for end users. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issues #1879 and #2114.*

**EMPLOYMENT PLAN OR STATUS UPDATE**
The script will now update the Employment Servicess Access Database for agencies collecting ES Referral stats. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2040.*

**LEP - SAVE**
Behind the scenes fixes to make the script run better and be more user friendly. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2127.*

**LTC - 5181**
Added case noting when the 'sent 5181 to case manager' check box is checked. Behind the scenes: updated the script end procedure message, and moved the stats block to the beginning of the script. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2118.*

**PROOF OF RELATIONSHIP**
Enhanced to support detailing multiple relationships and verifications at once, also will now autofill information from MAXIS into the script. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #1958.*

**RETURNED MAIL RECEIVED**
Information was added behind-the-scenes for statistics gathering purposes, and variable names were updated to be more descriptive. End users should not experience any change. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issues #2088 and #2091.*

**SIGNIFICANT CHANGE**
Changed denial reason "Income didn't decline at least 50% in the benefit month" to "Income did not decrease enough to qualify" since the policy on Significant Change is different from when the script was originally written. *Completed by Mel Fox (@MelissaFox-Stearns, Stearns County). Resolves issue #2035.*

===
### NOTICES SCRIPTS
**APPOINTMENT LETTER**
Added interview address for Carver County and for each of the MNPrairie locations (Dodge, Steele & Waseca Counties). *Completed by Ann Sunderman (@asunderman, Le Sueur County). Resolves issue #2070.*

**SEND NOMI**
Updated Hennepin County's Northwest regional office hours to reflect daily hours of 8 - 430. Also moved the stats block to the top of the script behind the scenes. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2108.*

**SNAP E&T LETTER**
Updated Hennepin County E&T time for the Central/NE region, and updated the E&T time, date, and location for the Northwest region. Also moved statistic information on the backend, cleaned up spelling errors, and removed the case note line regarding the manual referral if no manual referral has been made. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issues #2045 and #2105.*

===
### UTILITIES SCRIPTS
**TRAINING CASE CREATOR**
Note added to warn users that on MSA/SNAP cases the MSA grant may not be budgeted for the initial month of SNAP. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2044.*

Also, a redundant function was removed, end-users should not notice any changes. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2122.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Scripts retired in this release
===
### BULK SCRIPTS
**HOUSING GRANT FIATER**
Housing Grant FIATER was also removed as MAXIS does it now. *Removed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2083.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Functions Library (FuncLib) updates (for scriptwriters)
===
### New functions
**file_selection_system_dialog**
A new function for generating a file selection dialog using the system-default settings has been added. When this function is invoked, it will ask the user to browse to a file. That file is then passed to a variable, which can be used by your script. *Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issue #201.*

Usage example: `call file_selection_system_dialog(file_selected, file_extension_restriction)`

===
### Updated functions

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Other updates
===
### SETTINGS FILES
**TRAINING CASE SCENARIOS.xlsx**
Added an MSA case including MSA/HC/SNAP. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1964.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
===
### Contribution statistics ([day before previous release] to [day before current release])

<table>
    <tr>
        <th>Scriptwriter Name</th>
        <th>Agency</th>
        <th>Commits (Scripts)</th>
        <th>Commits (FuncLib)</th>
        <th>Commits (Total)</th>
    </tr>
    <tr>
        <td>Charles Potter</td>
        <td>Anoka County</td>
        <td>14</td>
        <td>0</td>
        <td><b>14</b></td>
    </tr>
    <tr>
        <td>David Courtright</td>
        <td>St. Louis County</td>
        <td>11</td>
        <td>0</td>
        <td><b>11</b></td>
    </tr>
    <tr>
        <td>Ilse Ferris</td>
        <td>Hennepin County</td>
        <td>11</td>
        <td>0</td>
        <td><b>11</b></td>
    </tr>
    <tr>
        <td>Robert Fewins-Kalb</td>
        <td>Anoka County</td>
        <td>6</td>
        <td>0</td>
        <td><b>6</b></td>
    </tr>
    <tr>
        <td>Veronica Cary</td>
        <td>DHS</td>
        <td>4</td>
        <td>0</td>
        <td><b>4</b></td>
    </tr>
    <tr>
        <td>Wendy LeVesseur</td>
        <td>Anoka County</td>
        <td>4</td>
        <td>0</td>
        <td><b>4</b></td>
    </tr>
    <tr>
        <td>Tim Delong</td>
        <td>Stearns County</td>
        <td>3</td>
        <td>0</td>
        <td><b>3</b></td>
    </tr>
    <tr>
        <td>Ann Sunderman*</td>
        <td>Le Sueur County</td>
        <td>2</td>
        <td>0</td>
        <td><b>2</b></td>
    </tr>
    <tr>
        <td>Laura Larson</td>
        <td>Olmsted County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
    <tr>
        <td>Casey Love</td>
        <td>Olmsted County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
