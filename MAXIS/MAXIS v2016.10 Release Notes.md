About this release
===
<<INFO ABOUT THE RELEASE WILL GO HERE>>

BlueZone Scripts are automatically updated via GitHub, without requiring any changes to files installed locally for counties and agencies. If you appear to be missing some of these updates, consider re-installing your scripts. Contact Charles.Potter@state.mn.us with any additional questions.

It is recommended that supervisors review these notes with staff. A PDF version of these notes is included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New scripts
===

### BULK
**REPT-INTR**
New Script that creates a report from REPT/INTR. Excel report generated with each item from INTR and a second worksheet with counts for each worker. Script includes the option to enter a supervisor X-Number and have all workers numbers listed under that supervisor checked. *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2573*

### DAIL
**WAGE MATCH SCRUBBER**
This new script helps workers process WAGE DAILs. The script grabs quarterly earnings information from the match as well as earned income information for the case and presents that information in an organized dialog to the financial worker. The script does not update or case note anything, but it does save the financial worker time and improves the accuracy of transcribing earned income information from the matches. *Completed by Robert Fewins-Kalb (@RoberT-1000 from Anoka County) Resolves Issue #2583*

### NOTES
**CASE DISCREPANCY**
Template for case noting information about a case discrepancy. EX: MAXIS/MMIS Discrepancy, ELIG discrepancy, etc. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2617*

**COUNTY BURIAL DETERMINATION**
New script that will case note a decision made on a County Burial Application. This script works in conjunction with the enhancements to County Burial Application Script - reading information from the case note created from that script. *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2585*

**GRH - NON-HRF-POSTPAY**
Case note script that will screen into non-hrf GRH cases and process GRH post payment. *Completed by Kenny Lee (@kennyasalee from Ramsey County) Resolves Issue #1730 and #2205*

### UTILITIES
**COPY CASE DATA FOR TRAINING**
 This script will grab case data from a training case and/or production cases, and will put the data into an Excel spreadsheet. For the script to run all the way through, you need to use a Training Case Creator template. The script is programmed to run with the data validation on the cells. *Completed by Robert Fewins-Kalb (@RoberT-1000 from Anoka County) Resolves Issue #1142*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### ACTIONS
**ABAWD BANKED MONTH FIATER**
Bug fixes to the script. The script will stop early in the run if the REVW date has not been entered and alert the worker to the reason for the error. The script also has a way to account for resources and handle adjusting the expedited status based on the information provided *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2491 & 2623*

**NEW JOB REPORTED**
Added TIKL checkbox, cleaned up date variables and case note, created more space/lined up edit boxes in dialog, added check for password in do loop *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2612*

### BULK
**DAIL REPORT**
The DAIL Report will now create a second worksheet in the Excel report that has counts for each worker's DAILs, including total DAILs and any of the DAIL types selected. *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2574*

**ES REFERRAL MISSING**
Fixes a bug that prevented the script from updating EMPS *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2597*

**SPENDDOWN REPORT**
Fix to the script to handle if there is a case on the caseload(s) that have no review date entered and if the caseload(s) have no cases that have a spenddown listed *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2614*

**REVW/MONT CLOSURES**
Adding logic to avoid case noting confusing lines about programs closing when those programs are not on the case. *Completed by Robert Fewins-Kalb (@RoberT-1000 from Anoka County) Resolves Issue #2565*

**REVS SCRUBBER**
Fixes a bug that causes an error at the end of the script run if no PRIV cases are found. *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2662*

### DAIL
**CSES SCRUBBER**
Will now case note the MEMB #, CS type, and the amount per person receiving CS. *Completed by Tim Delong (@StormageddonDLOA from Stearns County) Resolves Issue #2624*

Corrects a bug that sometimes prevented the script from updating UNEA panels in the correct footer month. *Completed by David Courtright (@courtrightd from St Louis) Resolves Issue #2646*

This resolves a bug that was preventing the script from completing the case note on certain SNAP / MFIP combination households. *Completed by David Courtright (@courtrightd from St Louis) Resolves Issue #2666*

**FINANCIAL ORIENTATION DATE MISSING**
Fixing error which prevent the script from starting. *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2581*

**NEW HIRE**
added CCA, ES, work number check boxes, added check for password in dialog do loop, removed msgboxes, added messages in script end procedure *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2612*

**NEW HIRE NDNH**
added CCA, ES, work number check boxes, added check for password in dialog do loop, removed msgboxes, added messages in script end procedure *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2612*

### NOTES
**CAF**
Several enhancements centered around the 'NOTES ON INCOME AND BUDGET" field: Moved the field closer to the other income fields, reordered income fields, updated error message text when the "NOTES ON INCOME AND BUDGET" field is not complete, and added trim function to ensure that users are entering information in this field. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2593*

**COUNTY BURIAL APPLICATION**
Update to the script that will autofill date of death and asset information from STAT. New fields for case noting additional detail including service type, place and amount. Place for contact person information. The script now has an option to create a Word Document with information about the application as much of this process happens outside of MAXIS. *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2577*

**CSR**
Now follows same logic as CAF, if the earned or unearned income fields have data entered the worker must input notes on income. *Completed by Robert Fewins-Kalb (@RoberT-1000 from Anoka County) Resolves Issue #2551*

**DENIED PROGRAMS**
This enhancement makes the script check for an additional line for ADDITIONAL APP when checking PND2. *Completed by Robert Fewins-Kalb (@RoberT-1000 from Anoka County) Resolves Issue #2642*

**EMERGENCY**
For Hennepin and Ramsey County users testing only - added EGA screening functionality to provide basic EMER programs information based on general criteria such as meeting residency, crisis reason and last issuance period. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2624*

**EXPEDITED SCREENING**
Corrected 10/16 utility deduction amount. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2570*

**HCAPP**
Gave agencies the option to have verification's needed at the top or the bottom of the case note (Similar to option in CAF). *Completed by Roy Walz (@RoyStearns from Stearns County) Resolves Issue #2606*

**HC RENEWAL**
Gave agencies the option to have verification's needed at the top or the bottom of the case note (Similar to option in CAF). *Completed by Roy Walz (@RoyStearns from Stearns County) Resolves Issue #2607*

**MFIP SANCTION AND DWP DISQUALIFICATION**
Added checkbox that will set a TIKL for each month of the six-month mandatory vendor period to remind workers to FIAT mandatory vendor info into ELIG results. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2596*

**PARIS MATCH**
Fixed bug that did not allow users to case note the information from the input dialogs. Also added more space for worker input in the dialog. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2598*

### NOTICES
**SNAP E AND T LETTER**
FOR HENNEPIN COUNTY USERS ONLY: removed date restriction for using the Somali language orientation, and updated verbiage on how users select this option. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2599*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Scripts retired in this release
===
### NOTES
**GRH - HRF**
GRH program no longer uses HRF forms so script is being retired. *Completed by Charles Potter(@Cdpotter from DHS). Resolved #2514*

**SNAP CASE REVIEW**
Hennepin County specific script removed per Hennepin County. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2605*

**SUBMIT CASE FOR SNAP REVIEW**
Hennepin County specific script removed per Hennepin County. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2605*

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
        <td><b>David Courtright</b></td>
        <td>St Louis</td>
        <td>3</td>
    </tr>
    <tr>
        <td><b>Tim Delong</b></td>
        <td>Stearns</td>
        <td>1</td>
    </tr>
    <tr>
        <td><b>Ilse Ferris</b></td>
        <td>Hennepin</td>
        <td>26</td>
    </tr>
     <tr>
        <td><b>Robert Fewins-Kalb</b></td>
        <td>Anoka</td>
        <td>10</td>
    </tr>
    <tr>
        <td><b>Kenny Lee</b></td>
        <td>Ramsey</td>
        <td>2</td>
    </tr>
     <tr>
        <td><b>Casey Love</b></td>
        <td>Ramsey</td>
        <td>26</td>
    </tr>
    <tr>
        <td><b>Charles Potter</b></td>
        <td>DHS</td>
        <td>3</td>
    </tr>
    <tr>
        <td><b>Roy Walz</b></td>
        <td>Stearns</td>
        <td>2</td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
