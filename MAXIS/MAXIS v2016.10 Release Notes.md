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
**GRH - NON-HRF-POSTPAY**
Case note script that will screen into non-hrf GRH cases and process GRH post payment. *Completed by Kenny Lee (@kennyasalee from Ramsey County) Resolves Issue #1730 and #2205*

### UTILITIES
**COPY CASE DATA FOR TRAINING**
 This script will grab case data from a training case and/or production cases, and will put the data into an Excel spreadsheet. For the script to run all the way through, you need to use a Training Case Creator template. The script is programmed to run with the data validation on the cells. *Completed by Robert Fewins-Kalb (@RoberT-1000 from Anoka County) Resolves Issue #1142*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### BULK
**DAIL REPORT**
The DAIL Report will now create a second worksheet in the Excel report that has counts for each worker's DAILs, including total DAILs and any of the DAIL types selected. *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2574*

**REVW/MONT CLOSURES**
Adding logic to avoid case noting confusing lines about programs closing when those programs are not on the case. *Completed by Robert Fewins-Kalb (@RoberT-1000 from Anoka County) Resolves Issue #2565*

### DAIL
**FINANCIAL ORIENTATION DATE MISSING**
Fixing error which prevent the script from starting. *Completed by Casey Love(@C-Love from Ramsey County) Resolves Issue #2581*

### NOTES
**CSR**
Now follows same logic as CAF, if the earned or unearned income fields have data entered the worker must input notes on income. *Completed by Robert Fewins-Kalb (@RoberT-1000 from Anoka County) Resolves Issue #2551*

**EXPEDITED SCREENING**
Corrected 10/16 utility deduction amount. *Completed by Ilse Ferris (@IlseFerris from Hennepin County) Resolves Issue #2570*



--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Scripts retired in this release
===
### NOTES
**GRH - HRF**
GRH program no longer uses HRF forms so script is being retired. *Completed by Charles Potter(@Cdpotter from DHS). Resolved #2514*

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
        <td><b>Ilse Ferris</b></td>
        <td>Hennepin</td>
        <td>2</td>
    </tr>
     <tr>
        <td><b>Robert Fewins-Kalb</b></td>
        <td>Anoka</td>
        <td>9</td>
    </tr>
    <tr>
        <td><b>Kenny Lee</b></td>
        <td>Ramsey</td>
        <td>2</td>
    </tr>
     <tr>
        <td><b>Casey Love</b></td>
        <td>Ramsey</td>
        <td>9</td>
    </tr>
    <tr>
        <td><b>Charles Potter</b></td>
        <td>DHS</td>
        <td>3</td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
