About this release
===
This BlueZone Scripts release was larger than usual, with four new scripts (including a banked months report script by Casey Love from Ramsey County and Ilse Ferris from Hennepin County) and over two dozen enhancements. In addition, several project-wide enhancements were made to remove outdated functions and streamline script workflows. As a result, county-specific scripts may see occasional message boxes warning of depreciated functions. If your agency experiences pop-ups, make sure you've updated your scripts, per the SIR announcement from May 12.

It is recommended that supervisors review these notes with staff. A PDF version of these notes is included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New scripts
===
### ACTIONS SCRIPTS
**LTC - ICF-DD DEDUCTION FIATER**
New script will FIAT earned income disregards on STAT/WKEX for LTC clients in ICF-DD's that receive earned income. Deductions will be FIATed for a selected month through the active budget period. *Completed by May Xiong (@mxiong1, Ramsey County) and Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2057.*

===
### BULK SCRIPTS
**BANKED MONTHS REPORT**
New script to create a report for submitting used Banked Months to DHS. This script will take a list from a specific Excel File of client data to review for reporting. The script then:
  1. Uses the case number and client name to confirm the correct client is found'
  2. Gathers the PMI
  3. Checks ELIG to ensure SNAP was open for this client in the report month
  4. Confirms SNAP was not prorated
  5. Checks for some basic ABAWD exemptions in the report month
  6. Reviews WREG to ensure it is coded correctly
  7. Counts the Initial ABAWD counted months and creates a list of these months
  8. Counts the 2nd Pd of ABAWD months (if used) and creates a list of these months
  9. If Requested, adds a Person Note to document the Banked Month being reported

With all of this detail the script adds all of the relevant information to the specific Excel file with the DHS report data for any client that still appears to have used a Banked Month in the report month. A second report will be created to detail any client not added to the DHS report, along with the reasons why this client was not added. 

This script requires a specific format of the Excel Files. The templates are available and should be saved in a local file location.

*Completed by Casey Love (@C-Love, Ramsey County) and Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2146.*

===
### NOTICES SCRIPTS
**ELIGIBILITY NOTIFIER**
This script will send a SPEC/MEMO to the client to notify them of potential eligibility for MA, MSP, MNSure, SNAP, or cash programs. It also contains information regarding how to apply, and CAF1 importance. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issues #2153, #2151, and #2171.*

**MA INMATE APPLICATION WCOM**
Adds a SPEC/WCOM to an MA approval notice to inform clients who have applied for MA (while in the process of being released from a correctional facility) of their MA start date. This start date is determined by trying to read the FACI panel for a release date. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issues #2148 and #2219.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### ACTIONS SCRIPTS
**ABAWD BANKED MONTHS FIATER**
Resolves a bug that caused the script to stop on UNEA panels with $0 coded on the SNAP PIC. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2177.*

**CASE TRANSFER**
When sending a SPEC/MEMO with new worker information, the script will now check if notices are to be sent to an AREP or Social Worker, and send copies of the memo if needed. It also case notes the action. Also, a minor bug was also corrected that prevented sending the memo when transferring a privileged case. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2227.*

**MA-EPD EI FIATER**
Script can now handle change in position of HC income estimator. Script can do this as well as current location of estimator to make the transition to the new panel more smooth if both version are available at the same time. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2242.*

**PAYSTUBS RECEIVED**
Script can now handle change in position of HC income estimator. Script can do this as well as current location of estimator to make the transition to the new panel more smooth if both version are available at the same time. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2242.*

**TRANSFER CASE**
The script now takes the user name (for in county transfers) and checks REPT/USER to find the new worker's contact information and enters it into the MEMO. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2242.*

===
### BULK SCRIPTS
**CASE NOTE FROM LIST**
The script was updated to replace the Excel file browser with the Windows standard file browser, which contains logic for looking at recent places, favorite locations, and multiple shared drives. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2008.*

**DAIL REPORT**
The script was enhanced to allow users to select which type of DAIL message to add to the DAIL report. The default selection will remain "All" DAIL messages. Also on the back end: updated the functionality to allow users to enter their password if they have been 'passworded' out, and moved statistical information to the top of the script per new guidelines. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2136.*

**FIND MAEPD MEDI CEI**
Functions were removed from this script and moved to the Functions Library. End users shouldn't notice any changes. An error with multicounty agencies and proper use of this function was also repaired. *Completed by Veronica Cary (@theVKC, DHS). Resolves issues #2232 and #2223.*

**FIND PANEL UPDATE DATE**
Added PACT, PARE, PBEN, STWK and WREG options to the script. Users can now search these MAXIS screens for updated dates based on time perimeters selected in the initial dialog. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issues #2130 and #2222.*

**MEMO FROM LIST**
The script was updated to replace the Excel file browser with the Windows standard file browser, which contains logic for looking at recent places, favorite locations, and multiple shared drives. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2008.*

**TIKL FROM LIST**
The script was updated to replace the Excel file browser with the Windows standard file browser, which contains logic for looking at recent places, favorite locations, and multiple shared drives. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2008.*

**UPDATE EOMC LIST**
The script was updated to replace the Excel file browser with the Windows standard file browser, which contains logic for looking at recent places, favorite locations, and multiple shared drives. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2008.*

Also, a bug was fixed which was causing the script to update the list with incorrect case statuses. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2181.*

===
### DAIL SCRUBBER SCRIPTS
**ABAWD FSET EXEMPTION CHECK**
The script will now display the results of the ABAWD/FSET Exemption Check. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #2163.*

**NEW HIRE**
When a client gets a new hire and someone else has used their SSN the names do not match. The script was not reviewing these inconsistencies. Now the script will pause if the names are not identical and give the user a chance to review the information and stop the script if necessary. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2179.*

**NEW HIRE NDNH**
When a client gets a new hire and someone else has used their SSN the names do not match. The script was not reviewing these inconsistencies. Now the script will pause if the names are not identical and give the user a chance to review the information and stop the script if necessary. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2179.*

**SEND NOMI**
Updated script to reflect Hennepin County's NW office opening at 8:00 a.m. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2168.*

===
### NOTES SCRIPTS
**APPROVED PROGRAMS**
The script now wraps up on SPEC/WCOM, as the user is instructed to check SPEC/WCOM for notice clarity. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2134.*

**BURIAL ASSETS**
Script will no longer require input when NONE is selected as burial agreement type, it also allows users to write their own burial agreement type. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2239.*

**CLIENT TRANSPORTATION COSTS**
A variable was fixed which was defined incorrectly. County-specific logic for Wabasha County should now be working correctly. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2231.*

**CLOSED PROGRAMS**
Did a general update of the script which includes the following...

1. Added informative text to the dialog box.
2. Tightened/cleaned up the dialog box for easier readability.
3. Added navigation buttons to the Insurance Affordability and Health Care Program manuals to the dialog box.
4. Removed functionality related the health care REIN dates from the script.
5. Added information to the end script message box regarding removal of HC REIN information.
6. Updated logic around future intake dates that became a bug when scripts were updated.

*Completed by Laura Larson (@LaLarson, Olmsted County). Resolves issue #2076.*

**DENIED PROGRAMS**
This update prevents the script from duplicating the reason for "Coding for denial" when case noting. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #2141.*

**EXPEDITED DETERMINATION**
Fixes the 'String Error' that was causing the script to stop before completion on some cases. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #2154.*

**FOSTER CARE HCAPP**
Actions taken wasn't case noting, but now it is. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #2182.*

**GOOD CAUSE CLAIMED**
Corrected the lower case name to all caps for statistical tracking. End users should not notice any changes. *Completed by Gay Sikkink (@GayS, Stearns County). Resolves issue #2031.*

**MFIP TO SNAP TRANSITION**
Corrected a minor bug that may have caused the script to read the incorrect footer month in MAXIS. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2228.*

===
### NOTICES SCRIPTS
**MFIP ORIENTATION**
Added a list of agency office addresses within the script to correct an issue with the address auto-fill in the dialog. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2140.*

**NOMI**
Updated script to reflect Hennepin County's NW office opening at 8:00 a.m. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2168.*

**POSTPONED WREG VERIFS**
Script will now TIKL for the next cutoff date to close case. Since this script is designed for the postponed WREG verification workaround we are supposed to close the case in accordance with expedited processing. This means sometimes closing cases before a ten day period to turn in verifications (to meet cutoff requirements). See TE02.05.70.01 for details. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2123.*

**SNAP E AND T LETTER**
Added "other manual referral" option to the "manual referral needed" droplist. The "other manual referral notes" is a mandatory field if the 'manual referral' option is selected. This field will be notes added to the manual referral. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2174.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Functions Library (FuncLib) updates (for scriptwriters)
===
### UPDATED FUNCTIONS
**add_JOBS_to_variable**
Function is being updated to account for shift to HC income estimator. This will allow a smooth transition while it's possible both version of the panel are available. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves FuncLib issue #227.*

**autofill_editbox_from_MAXIS**
Fixed bug in function that outputs ABAWD information into scripts such as NOTES - CAF and NOTES - CSR. Also enhanced the function to include a list of the counted ABAWD and second set of ABAWD months when ABAWD status in STAT/WREG is coded as a "10", and includes the second set of ABAWD months when ABAWD status in STAT/WREG is coded as a "11". *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #196.*

**cancel_confirmation**
Updated the `cancel_confirmation` function to replace the `StopScript` portion of the function with `script_end_procedure`, and added a new closing message indicating it's a cancellation. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #211.*

**script_end_procedure**
The `script_end_procedure` has a new feature - if `disable_StopScript` is set to `true`, the function will keep running and not stop the script, allowing chain-loading with ease. *Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issue #205.* 

Also updated `script_end_procedure` to bypass the closing message if being used in scripts where it comes from `cancel_confirmation`. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #211.*

**MAXIS_dialog_navigation**
Added WKEX panel navigation to the `MAXIS_dialog_navigation` function. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #213.*

**write_panel_to_MAXIS_JOBS**
Function is being updated to account for shift to HC income estimator. This will allow a smooth transition while it's possible both version of the panel are available. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves FuncLib issue #227.*

===
### NEW FUNCTIONS
**CM_plus_2_mo** and **CM_plus_2_yr**
Added current-month-plus-two month and year to the list of global constant dates. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #222.*

**get_county_code**
`worker_county_code_determination` has been depreciated, and a new simplified function called `get_county_code` has replaced it. Scriptwriters should use `get_county_code` any time county-specific functionality (such as x1 numbers, custom addresses, or custom dialogs) is implemented. *Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issue #208.*

**income_test_SNAP_categorically_elig**
This new function determines the categorically eligible income limit for SNAP cases based on the household size. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves FuncLib issue #191.*

**income_test_SNAP_gross**
This new function determines the gross income limit for SNAP cases based on the household size. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves FuncLib issue #191.*

**income_test_SNAP_net**
This new function determines the net income limit for SNAP cases based on the household size. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves FuncLib issue #191.*

**navigate_to_MMIS**
Added `navigate_to_MMIS` function to be used when navigating from one BlueZone function to another (MAXIS, PRISM, INFOPAC, etc.) *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #192.*

**navigate_to_MAXIS**
Added `navigate_to_MAXIS` function to be used when navigating from one BlueZone function to another (MMIS, PRISM, INFOPAC, etc.) *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #193.*

**ten_day_cutoff_check**
This new function determines the ten-day cutoff date, and has been updated for 2016. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves FuncLib issue #191.*


--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Other updates
===
**BULK - BULK SCRIPT TEMPLATE.vbs**
A template for scriptwriters to use as a starting point for developing custom bulk scripts has been completed. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2167.*

**OLD MAIN MENU SCRIPTS**
Three old MAIN MENU scripts (MEMOS, NOTES 0-G, and NOTES H-Z) have had depreciation notices added. Users seeing these pop-ups should ask a scripts administrator to update their scripts with the latest version immediately. Access to these old main menus expires in the June release. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2193.*

**REDIRECT - NOTES H-Z.vbs**
An old redirect file was removed. End users should not notice any issues with this. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2208.*

**SETTINGS - GLOBAL VARIABLES.vbs**
The `county_name` variable was removed from Global Variables, as the new function `get_county_code` determines this programmatically. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #2145.*

**ALL SCRIPTS**
The following functions were depreciated across all scripts:

* `ERRR_screen_check` was integrated into other functions and is no longer supported
* `maxis_check_function` has become `check_for_MAXIS`.
* `navigate_to_screen` has become `navigate_to_MAXIS_screen`.
* `write_editbox_in_case_note` has become `write_bullet_and_variable_in_CASE_NOTE`.
* `write_new_line_in_case_note` has become `write_variable_in_CASE_NOTE`.
* `write_new_line_in_SPEC_MEMO` has become `write_variable_in_SPEC_MEMO`.
* `worker_county_code_determination` has become `get_county_code`, and several scripts have added this function to improve operations across multicounty agencies.
* `write_TIKL_function` has become `write_variable_in_TIKL`.

In addition, in order to meet feature parity with the separate (and county-driven-not-state-supported) PRISM script project, several MAXIS-specific variables were renamed:

* `case_number` has become `MAXIS_case_number`
* `footer_month` has become `MAXIS_footer_month`
* `footer_year` has become `MAXIS_footer_year`

Finally, the Functions Library block and statistics block were updated to take up less space and be cleaner code-wise.

They were removed (or renamed) from the primary script directory, and modified in Functions Library to generate a pop-up box if they are invoked. End users should not notice any changes because of this, aside from any county-specific scripts that use these depreciated functions. Scriptwriters experiencing these functions should update them immediately. *Completed by Veronica Cary (@theVKC, DHS). Resolves issues #2195, #2223, and #1938, as well as FuncLib issues #71, #106, and #184. Gay Sikkink (@GayS, Stearns County) assisted with the conversion of actions scripts.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
===
### Contribution statistics (04/24/2016 to 05/24/2016)

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
        <td>497</td>
        <td>7</td>
        <td><b>504</b></td>
    </tr>
    <tr>
        <td>Ilse Ferris</td>
        <td>Hennepin County</td>
        <td>23</td>
        <td>20</td>
        <td><b>43</b></td>
    </tr>
    <tr>
        <td>Charles Potter</td>
        <td>Anoka County</td>
        <td>19</td>
        <td>2</td>
        <td><b>21</b></td>
    </tr>
    <tr>
        <td>Gay Sikkink</td>
        <td>Stearns County</td>
        <td>17</td>
        <td>0</td>
        <td><b>17</b></td>
    </tr>
    <tr>
        <td>Casey Love</td>
        <td>Ramsey County</td>
        <td>8</td>
        <td>0</td>
        <td><b>8</b></td>
    </tr>
    <tr>
        <td>David Courtright</td>
        <td>St. Louis County</td>
        <td>8</td>
        <td>0</td>
        <td><b>8</b></td>
    </tr>
    <tr>
        <td>Robert Fewins-Kalb</td>
        <td>Anoka County</td>
        <td>3</td>
        <td>2</td>
        <td><b>5</b></td>
    </tr>
    <tr>
        <td>Laura Larson</td>
        <td>Olmsted County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
    <tr>
        <td>May Xiong*</td>
        <td>Ramsey County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
