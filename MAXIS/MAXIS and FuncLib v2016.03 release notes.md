About this release
===
The March 2016 BlueZone Scripts is an update release, without many new scripts. One new script which will be exciting for agencies is the long-awaited Training Case Creator utilities script. We've also added a new bulk list and two new case note scripts, and a new script to create a list of all POLI TEMP topics. There were several enhancements and bug fixes released for existing scripts as well.

It is recommended that supervisors review these notes with staff. A PDF version of these notes is included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New scripts
===
### Bulk scripts
**Update EOMC List**
This script will check all cases on a saved REPT/EOMC Excel file from a previous month and update the file with current status for each program. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #657.*

### Notes scripts
**Good Cause Claimed**
A template to record determination results from a Good Cause Request. *Completed by Gay Sikkink (@GayS, Stearns County). Resolves issue #1985.*

**Returned Mail Received**
This script case notes the details of the address received from, new address (if one is known), county of new address (if applicable), if returned mail was resent to the client, if forms were sent to the client, if the client has a MNsure case, the MNsure number if applicable, if the MNsure case has the correct address, and misc notes/actions taken. Automatically capitalizes the address (old and new) and the county when case noted. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issue #1993.*

### Utilities scripts
**POLI/TEMP List**
New script that will create an Excel spreadsheet with current POLI TEMP topics, temp reference and revised date. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1952.*

**Training Case Creation**
This new script can create training cases en masse for a selection of workers. Can APPL, add panels, approve results, and transfer cases. Requires an Excel file (which contains scenarios) which can be downloaded at the link below (press "view raw" to download the scenarios file).

Scenarios download link: https://github.com/MN-Script-Team/DHS-MAXIS-Scripts/blob/RELEASE/Script%20Files/SETTINGS%20-%20TRAINING%20CASE%20SCENARIOS.xlsx

*Completed by Veronica Cary (@theVKC, DHS), Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County), Charles Potter (@CDPotter, Anoka County), Ilse Ferris (@IlseFerris, Hennepin County), Casey Love (@C-Love, Ramsey County), David Courtright (@courtrightd, St. Louis County), and Lucas Shanley (@lpshanley, St. Louis County). Resolves issue #53.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### Actions scripts
**ABAWD Banked Months FIATer**
Fixes a bug that was causing errors on cases with ended UNEA income. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2018.*

**Housing Grant FIATer**
Enhancement to the script includes handling for either a single month or multiple months (up to current month plus one). Also updated dialog box, and updated the statistical information. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issues #1963 and #2006.*

**Paystubs Received**
Script has been enhanced to case note the PIC correctly if more then 4 pay stubs are being used in the script. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1891.*

**Transfer Case**
Verbiage added to final message box reminding worker to send case file. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1956.*

**Multiple scripts**
ABAWD Screening Tool, New Job Reported, and Paystubs Received were updated to enhance the "passworded out" handling, optimizing this for users running BlueZone version 6+. This prevents issues where the pop-up box (warning the user about being locked out of MAXIS) prevents the user from re-entering their password. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #1977.*

===
### Bulk scripts
**COLA Auto Approved DAIL Noter**
Script was missing message boxes which prevented proper function at times. Corrected error, script runs smoothly now. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1928.*

**REVS List**
Updated some internal variables to make sure script doesn't derail for computers that define the date constant without preceding zeroes ("3/16/2016" vs "03/16/2016"). *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #2014.*

**REVW/MONT Closures**
Changed "Client needs to reapply for (PROGRAM) on (DATE)" to "Client needs to turn in new application for (PROGRAM) on (DATE)" to be more clear as to client responsibility and reapplication processing guidelines. The script now looks similar to the NOTES - CLOSED PROGS verbiage. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1968.*

**Main Menu**
The functionality which generates the buttons was updated. This should not affect users. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1889.*

===
### DAIL Scrubber scripts
**Citizenship Verified**
This script has been updated to require that the user select the specific household members to update, instead of the household members to not update. The script will not allow you to continue until you have selected at least one household member, and those member(s) should be listed on DAIL/DAIL. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #1967.*

**New Hire** and **New Hire NDNH**
Now, When the script enters a JOBS panel, it checks for the "This Information will expire ..." message which indicates that the JOBS panel will not carry forward to the next footer month. When this happens the script will now give you a pop-up to alert the worker to check the next footer month. *Completed by Mel Fox (@MelissaFox-Stearns, Stearns County). Resolves issue #1821.*

Also, handling has been added for accounting for a DAIL update where it will sometimes say "UNKNOWN" as the hire date instead of an actual date. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issue #1984.*

**Send NOMI**
Changed way script reads TIKL by just reading entire date and time in one line and making it one variable. This should resolve issues where the date is formatted in non-standard ways. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1970.*

===
### Notes scripts
**Approved Programs**
Script will no longer search for SNAP or cash results if the user does not select the program checkboxes. It will also no longer case note unselected program results. Also, the WCOM is no longer needed, as MAXIS now handles the CS disregard notice properly. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issues #1935 and #1981.*

Also, a bug was corrected that created an error message when attempting to update the banked month Access database for cases with less than 3 months or multiple banked month members. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #1943.*

**CAF**
An issue with the variable name for footer month was causing WREG counted-months not to pull correctly. This has been resolved. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1941.*

A checkbox was added to indicate an interpreter was used for the CAF interview. *Completed by Mel Fox (@MelissaFox-Stearns, Stearns County). Resolves issue #1979.*

Enhanced script with error handling if CAF is more than 30 or 45 days old and TIKL for denial is checked. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #1982.*

**Change Reported**
Added the checkbox to the dialog for baby born asking if the babys managed health care plan has been updated to match the mothers. Also updated variables to allow "actions taken" to case note correctly in the HH Comp section of the script. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issues #1955 and #2011.*

**Closed Programs**
Added checkbox for sending DHS-5181 to the case manager. *Completed by Gay Sikkink (@GayS, Stearns County). Resolves issue #1962.*

**Combined AR**
Updated the dialog and the case note portion of the script to add the eDRS checkbox and case note that it was checked. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issue #1953.*

**Explanation of Income Budgeted**
Enhanced script to separate Self Employment income from other earned income and provides message about self employment policy. New field added to call out information about Overtime Income explanation. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issues #1806 and #1917.*

**Foster Care HCAPP**
Tightened up the dialog box for better viewing on smaller screens, and added information/instructional text. *Completed by Laura Larson (@LaLarson, Olmsted County). Resolves issue #1939.*

**HC Renewal**
Several enhancements to this script have been made including specified error handling for users that miss mandatory fields in the main dialog (users will be informed of which field was missed), footer month/year navigation to correct an issue with users selecting a footer month that wasn't current month plus one, added a 'MMIS updated' checkbox and added the field "cost effective insurance availability to the dialog. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issues #1922, #1923, and #1925.*

**LEP - Sponsor Income**
Updated the constants for the 2016 sponsor income limits. See: CM0019.06. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #1975.*

**LTC - 1503**
Script wasn't able to go into edit mode on HCMI. Added in functionality. Moved check for maxis so script doesn't nav to stat/faci immediately after dialog without checking. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1919.*

Added checkbox for sending DHS-5181 to the case manager. *Completed by Gay Sikkink (@GayS, Stearns County). Resolves issue #1962.*

**LTC - Asset Assessments**
Added checkbox for sending DHS-5181 to the case manager. *Completed by Gay Sikkink (@GayS, Stearns County). Resolves issue #1962.*

**LTC - MA Approval**
Added checkbox for sending DHS-5181 to the case manager. *Completed by Gay Sikkink (@GayS, Stearns County). Resolves issue #1962.*

**LTC - Renewal**
Added checkbox for sending DHS-5181 to the case manager. *Completed by Gay Sikkink (@GayS, Stearns County). Resolves issue #1962.*

**MFIP Sanction and DWP Disqualification**
Makes it so that when you select add a WCOM that the script actually is able to add the WCOM. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issue #1948.*

**Main Menu**
Reorganized NOTES main menu into alphabetical order, and corrected a broken link to the SIR script wiki. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1900.*

Also expanded some acronyms so descriptions are a bit more clear. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1972.*

**Multiple scripts**
Multiple NOTES scripts were updated to enhance the "passworded out" handling, optimizing this for users running BlueZone version 6+. This prevents issues where the pop-up box (warning the user about being locked out of MAXIS) prevents the user from re-entering their password. Those scripts are:
* Approved Programs
* Change Report Form Received
* Change Reported
* Client Contact
* Closed Programs
* Combined AR
* CSR
* Denied Programs
* Documents Received
* Emergency
* Expedited Determination
* HC Renewal
* HCAPP
* HRF
* Interview Completed
* MFIP to SNAP Transition
* MTAF
* Overpayment
* Verifications Needed

*Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #1977.*

===
### Notices scripts
**Appointment Letter**
Added restriction for Hennepin County users. Restriction previously found in MEMOS - MAIN MENU, and has been moved to the script itself. Also updated address for Goodhue County. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issues #1932 and #1987.*

Script was updated to enhance the "passworded out" handling, optimizing this for users running BlueZone version 6+. This prevents issues where the pop-up box (warning the user about being locked out of MAXIS) prevents the user from re-entering their password. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #1977.*

**MFIP Orientation**
Corrects a bug that was preventing user-entered addresses from displaying on the memo sent to clients. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #2012.*

**NOMI**
Added handling for sending the MEMOS to SWKR's and AREP's in addition to the applicant/recipient if they have a SWKR and/or AREP that receives notices. Additional enhancements (Hennepin County only) include:

* Northwest office hours end time change from 5:00 to 4:30.
* Added checkbox/memo verbiage for if the HH has applied for MFIP/DWP, and requires a face-to-face interview.
* Added a button to link to the internal HSR manual NOMI page.
* Added automatic TIKLs to follow up on the NOMIs sent.

*Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #2022 and #2023.*

**SNAP E&T Letter**
Restricted access to Mahnomen county from using the SNAP E & T Letter and the ABAWD Banked months FIATer as they are an exempt county. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1888.*

**Main Menu**
Updated the NOTICES SIR instructions link to point to the NOTICES section of the SIR script wiki. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1899.*

Also, the functionality which generates the buttons was updated. This should not affect users. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1889.*

### Utilities scripts
**Info**
Scriptwriter Laura Larson has moved from Goodhue County to Olmsted County, so her contact information has been updated. *Completed by Laura Larson (@LaLarson, Olmsted County). Resolves issue #1940.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Scripts retired in this release
===
### Actions scripts
**CS Disregard FIAT**
Retired script as MAXIS has been updated to handle processing of these cases. Users will no longer need to manually FIAT eligibility. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1978.*

===
### Notices scripts
**CS Disregard WCOM**
Retired script as MAXIS has been updated to handle processing of these cases. Users will no longer need to manually FIAT eligibility. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1980.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Functions Library (FuncLib) updates (for scriptwriters)
===
### Updated functions
**Autofill Editbox from MAXIS**
Scripts can now autofill if more than 9 active asset panels exist. This applies to ACCT, CARS, OTHR, REST, and SECU. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves FuncLib issue #190.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Other updates
===
**GLOBAL VARIABLES.vbs**
A slash was added to the `script_repository` variable if `run_locally` is set to true. This makes the `script_repository` logic match other scripts when testing DAIL Scrubber enhancements. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #1965.*

**LAST UPDATE DATE.txt**
A "LAST UPDATE DATE.txt" file was created which will store the last updated date for Global Variables or Power Pads. This will be updated periodically to gently remind people to occasionally update their scripts when new Global Variables or Power Pad updates are available. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #1908.*

**README.md**
The release notes link in the readme has been updated, and a reference to our Slack team has been added. *Completed by Veronica Cary (@theVKC, DHS). Resolves issues #1866 and #1918.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
===
### Contribution statistics (02/22/2016-03/27/2016)

<table>
    <tr>
        <th>Scriptwriter Name</th>
        <th>Agency</th>
        <th>Commits (Scripts)</th>
        <th>Commits (FuncLib)</th>
        <th>Commits (Total)</th>
    </tr>
    <tr>
        <td>Casey Love</td>
        <td>Ramsey County</td>
        <td>26</td>
        <td>0</td>
        <td><b>26</b></td>
    </tr>
    <tr>
        <td>Ilse Ferris</td>
        <td>Hennepin County</td>
        <td>18</td>
        <td>0</td>
        <td><b>18</b></td>
    </tr>
    <tr>
        <td>Tim Delong</td>
        <td>Stearns County</td>
        <td>12</td>
        <td>0</td>
        <td><b>12</b></td>
    </tr>
    <tr>
        <td>Charles Potter</td>
        <td>Anoka County</td>
        <td>9</td>
        <td>3</td>
        <td><b>12</b></td>
    </tr>
    <tr>
        <td>Veronica Cary</td>
        <td>DHS</td>
        <td>10</td>
        <td>0</td>
        <td><b>10</b></td>
    </tr>
    <tr>
        <td>Gay Sikkink</td>
        <td>Stearns County</td>
        <td>8</td>
        <td>0</td>
        <td><b>8</b></td>
    </tr>
    <tr>
        <td>David Courtright</td>
        <td>St. Louis County</td>
        <td>6</td>
        <td>0</td>
        <td><b>6</b></td>
    </tr>
    <tr>
        <td>Laura Larson</td>
        <td>Olmsted County</td>
        <td>2</td>
        <td>0</td>
        <td><b>2</b></td>
    </tr>
    <tr>
        <td>Melissa Fox</td>
        <td>Stearns County</td>
        <td>2</td>
        <td>0</td>
        <td><b>2</b></td>
    </tr>
    <tr>
        <td>Robert Fewins-Kalb</td>
        <td>Anoka County</td>
        <td>2</td>
        <td>0</td>
        <td><b>2</b></td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
