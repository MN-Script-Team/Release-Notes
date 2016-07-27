About this release
===
The February 2016 update for BlueZone Scripts is a very large release; one of the largest releases we've ever completed. It is the first release since a script freeze was lifted in January, so there are many new scripts that have been "in development" for a while. We have several brand new scripts, including multiple scripts focusing on foster care for MAXIS workers, a TYMA TIKLer, several new BULK action scripts, and many scripts which condense older scripts. In addition, the "MEMOS" button has been replaced with a "NOTICES" button (accessible if you reinstall your scripts with the latest installer, which is also now available). All together:

* 19 new scripts are available
* 17 existing scripts were updated
* 7 existing scripts were retired (combined into new scripts)
* 5 new scriptwriter functions or constants were introduced
* 3 new scriptwriters participated (from Hennepin, Olmsted, and Washington Counties)

It is recommended that supervisors review these notes with staff. A PDF version of these notes is included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New scripts
===
### Actions scripts
**TYMA TIKLer** <br>
A script for TIKLing for return of TYMA report forms. Can be configured to send all TIKLs at once or merely TIKLing the first message. This can be configured with the Global Variables file, and will default to TIKLing the first message only. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1754.*

===
### Bulk scripts
**Case Note From List** <br>
This new script can case note in bulk from either manual entry, REPT/ACTV, or an Excel spreadsheet of your choice. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issues #1569 and #1882.*

**NON MAGI HC INFO** <br>
This new script creates a list of cases with non-MAGI HC deductions. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1601.*

**Memo From List** <br>
This new script can memo in bulk from either manual entry, REPT/ACTV, or an Excel spreadsheet of your choice. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1569.*

**TIKL From List** <br>
This new script can TIKL in bulk from either manual entry, REPT/ACTV, or an Excel spreadsheet of your choice. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1569 and #1882.*

===
### DAIL scrubber scripts
**TYMA Scrubber** <br>
A script for processing the TIKLs created by the TYMA TIKLer script (a new actions script described elsewhere in this document). *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1792.*

===
### Navigation scripts
**Phone Number or Name Look Up** <br>
This new script combines the "Phone Number Look Up" and "REPT search" scripts into one script. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issue #1603.*

===
### Notes scripts
**Client Transportation Costs** <br>
This script combines the old "Gas Card Issued" and "Mileage Reimbursement" scripts, and adds a function for "Bus Tokens Issued".  Worker chooses how transportation funds were issued and completes the corresponding dialog and the script case notes information provided. *Completed by Mel Fox (@MelissaFox-Stearns, Stearns County). Resolves issue #1609.*

**EDRS Disqual Match Found** <br>
New notes scripts to walk worker through steps necessary when a SNAP recipient has an eDRS disqualification match. Procedure follows POLI/TEMP TE02.08.127. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #881.*

**Expedited Determination** <br>
New script that creates a detailed case note about how expedited was determined on a case. Includes actual case income/expenses and dates to detail timeliness.

**Foster Care HCAPP** <br>
This is a case note template for when a HCAPP is received for a foster care client. *Completed by Devonne Kent (@devonne01, Wright County). Resolves issue #1815.*

**Foster Care Review** <br>
This script case notes when a foster care review is received for Health Care. *Completed by Devonne Kent (@devonne01, Wright County). Resolves issue #1812.*

**HC ICAMA** <br>
This is a new basic case noting script to note details of a HC ICAMA action. *Completed by Kelly Hiestand (@khiestand, Wright County). Resolves issue #1816.*

**MSQ** <br>
This is a case note script that updates the STAT/ACCI panel when an MSQ form is not returned. It will case note the details. *Completed by Kelly Hiestand (@khiestand, Wright County). Resolves issue #1148.*

**OHP Received** <br>
This script is for when an out of home placement form is received. It will create a case note. *Completed by Devonne Kent (@devonne01, Wright County). Resolves issue #342.*

===
### Notices scripts
**ABAWD With Child In HH WCOM** <br>
Script will add a WCOM as prescribed in POLI/TEMP 02.05.70.30 when there is an adult in the SNAP HH and a child under 18 in the SNAP HH. Can write multiple people's names is allowed/needed. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1468.*

**Method B WCOM** <br>
New MEMOS script creates detailed WCOM regarding spenddown vs. recipient amount for method B HC cases. *Completed by Chris Johnson (@CJOHNS356, Olmsted County) and Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #599.*

===
### Utilities scripts
**Banked Month Database Updater** <br>
A utility to check and update the ABAWD Banked Month access database before submitting the monthly list. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #1787.*

**Update Worker Signature** <br>
Update Worker Signature is now a Utilities script. It can be found on the Utilities Main Menu (which is also crosslisted in the Actions Main Menu, in the top-right corner). *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #1612.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing scripts
===
### Actions scripts
**ABAWD Banked Months FIATer** <br>
Manual run times were added behind-the-scenes for statistics calculation purposes. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue  #1744.*

Also, a typo that was causing the phone deduction to be entered incorrectly on the garbage deduction line in FIAT was resolved, as was a bug that was causing the script to fail to enter shelter deductions into the budget on some cases. *Build by David Courtright (@courtrightd, St. Louis County). Resolves issues #1755 and #1831.*

**Paystubs Received** <br>
The script will now warn users when trying to enter a future paystub date. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1761.*

**Utilities Main Menu Button**
A new button that links to the "Utilities Main Menu" was added to the Actions menu. The UTILITIES Main Menu now contains the Update Worker Signature script and others. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #1835.*

===
### Bulk scripts
**Case Transfer** <br>
An issue where the script was transferring more cases than requested was fixed. Also fixed an error around comparing TANF Months, and conformed the entry of x1 numbers so that all 7 digits are required.' *Completed by Casey Love (@C-Love, Ramsey County). Resolves issues #1764, #1904, and #1905.*

**INAC Scrubber** <br>
The script was reading the wrong number of characters causing problems on case loads with more than 1 page of inactive cases ran by that user. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1774.*

**REVW/MONT Closures** <br>
The script was occasionally derailing due to an outdated method of going to case note. Added a newer function to fix this. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1759.*

**Main Menu** <br>
Corrected links in buttons for MEMO and TIKL from list. Correct a text bug on ADDR and the group box. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1880.*

===
### Notes scripts
**Approved Programs** <br>
A major rewrite of the script now case notes when programs have been approved with improved handling for multiple cash programs and documenting ABAWD banked months used. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issues #1663, #1262, and #1235.*

Additionally, functionality was added to allow counties to track ABAWD Banked Month usage by case number and member using a Microsoft Access database if desired. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issue #1785.*

*Assorted bug fixes on this enhancement were completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #1771.*

**CAF** <br>
A checkbox was added to indicate that the client is willing to work with E&T. Also rearranged the group of checkboxes in the dialog box to make room and put in alphabetical order. *Completed by Mel Fox (@MelissaFox-Stearns, Stearns County). Resolves issue #1805.*

Also corrected a bug causing the footer month/year navigation to fail, and added the form DHS-6696 as an option to select as a health care document submitted. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issues #1845 and #1830.*

A small typo in the checkbox area of the case note was corrected. *Completed by Katie Martini (@KateiMartini, Washington County). Resolves issue #1853.*

**Change Reported** <br>
The script was updated to remove "Baby's SSN" from the dialog box and case notes (in the Baby Born section). *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves issue #1768.*

The script has also been updated to correct a typo that is preventing it from running. *Completed by Robert Fewins-Kalb (@RobertFewins-Kalb, Anoka County). Resolves issue #1748.*

**Denied Programs** <br>
In some case note lines a duplicate colon existed. These duplicate colons have been removed. *Completed by Charles Clark (@senhorc, Hennepin County). Resolves issue #1801.*

**Employment Plan or Status Update** <br>
Corrected a bug with employment plan noting that was incorrectly notifying users that they needed to complete the school information field to continue. *Build by David Courtright (@courtrightd, St. Louis County). Resolves issue #1752.*

**HC Renewal** <br>
A new message box to remind the worker to update MMIS was added. *Completed by Devonne Kent (@devonne01, Wright County). Resolves issue #1238.*

**Interview Completed** <br>
Blanks out the CAF date if the date is more than 60 days old. *Completed by Casey Love (@C-Love, Ramsey County). Resolves issue #1604.*

**Main Menu** <br>
The Notes Main Menu has been completely rewritten to utilize automatic resizing and button placement. End users should notice no differences but scriptwriters can take advantage of an easier process for updating with new notes scripts. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #1828.*

A display glitch with the County Burial Application script (in the main menu) has been repaired. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1738.*



===
### Notices scripts
**SNAP E&T Letter** <br>
Several enhancements to this script include adding manual referral option for eligible students, updated verbiage about when a manual referral should be made, updated manual run time (for statistics-gathering agencies), an automatic TIKL option (to TIKL out for 30 day return of verification of E&T compliance), and added info to case notes for manual referral/TIKL information (if applicable). *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issues #1779, #1781, #1782, and #1789.*

Also, a bug was corrected that prevented the script from sending a letter when a single digit hour was entered for the appointment time. In addition, a typo that prevented the script from working for the Duluth office was corrected. *Completed by David Courtright (@courtrightd, St. Louis County). Resolves issues #1871 and #1872.*

**Main Menu** <br>
In addition to the new name for what used to be called the "MEMOS" section, the Main Menu was upgraded with a separate section for SNAP WCOMs. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1734.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Scripts retired in this release
===
### Actions scripts
**Update Worker Signature**
Update Worker Signature has been moved to the Utilities main menu. Agencies without the newest Power Pad (available by reinstalling your scripts) can still find this in the "UTILITIES" button on the Actions Main Menu. *Completed by Veronica Cary (@theVKC, DHS). Resolves issues #1612 and #1835.*

### Bulk scripts
**Bulk TIKLer** <br>
This script functionality has been replaced with a new script called *TIKL From List*. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1569.*

**Case Note From Excel List** <br>
This script functionality has been replaced with a new script called *Case Note From List*. *Completed by Charles Potter (@CDPotter, Anoka County). Resolves issue #1569.*

**PDED** <br>
This script functionality has been replaced with a new script called *NON-MAGI HC INFO*. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1601.*

**MISC. NON-MAGI HC Deductions** <br>
This script functionality has been replaced with a new script called *NON-MAGI HC INFO*. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #1601.*

### Navigation scripts
**Phone Number Look Up** <br>
This script has been retired and replaced with the new "Phone Number or Name Look Up" script. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves part of issue #1603.*

**REPT Search** <br>
This script has been retired and replaced with the new "Phone Number or Name Look Up" script. *Completed by Tim Delong (@StormageddonDLOA, Stearns County). Resolves part of issue #1603.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Other updates
===
### New/updated functions for scriptwriters
**autofill_editbox_from_MAXIS** <br>
Functionality added to autofill information from the SWKR panel. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue #179.*

**CM variables** <br>
New variables were added for current month and year (`CM_mo` and `CM_yr`), as well as the month and year in current month plus one (`CM_plus_1_mo` and `CM_plus_1_yr`). *Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issues 169 and 175.*

**Check_for_MMIS** <br>
A function to determine if you're currently in MMIS. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue 182.*

**MAXIS_footer_month_confirmation** <br>
A function for checking and changing the footer month to the MAXIS_footer_month & MAXIS_footer_year selected by the user in the initial dialog if necessary. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue 173.*

**write_panel_to_MAXIS_IMIG** <br>
Adding functionality to write codes to the bottom half of IMIG for the Training Case Creator. *Completed by Casey Love (@C-Love, Ramsey County). Resolves FuncLib issue #177.*

**Alphabetized Functions** <br>
Reordered functions to be in alphabetical order. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves FuncLib issue 181.*

**Depreciated beta blocking removed** <br>
Old safeguards to prevent beta repository usage by non-beta agencies were removed, as their functionality has been depreciated by the removal of the beta branches. *Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issue 170.*

**Old FuncLib block removed** <br>
The old FuncLib block example was removed from the functions library. *Completed by Veronica Cary (@theVKC, DHS). Resolves FuncLib issue 174.*

===
### Other file updates
**Global Variables** <br>
TYMA_TIKL_all_at_once has been added to the Global Variables file. The default behavior both in the script and the Global Variables file is to set this to false. Agencies installing or reinstalling scripts will be able to modify this variable in the installer. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #1794.*

**Power Pad** <br>
The "MEMOS" button has been changed to a "NOTICES" button. Agencies who update their scripts with the newest version of the installer should see a change in the Power Pad reflecting this. The old Power Pad will continue to work, as the MEMOS menu has been set to forward to the NOTICES menu. All MEMOS script names have been updated to reflect the change.

**README.md** <br>
The project README file was updated with current and helpful information for scriptwriters and non-scriptwriters alike. *Completed by Veronica Cary (@theVKC, DHS). Resolves issues #1778 and #1796.*

**Statistics folder** <br>
The "Statistics" folder (primarily for scriptwriters) has been replaced with a "Databases for script usage" folder. In addition, David Courtright's (St. Louis County's) database for tracking ABAWD months was added, and the Global Variables file adjusted to compensate for these new paths. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #1849.*

===
### Contribution statistics (01/24/2016-02/22/2016)

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
        <td>58</td>
        <td>2</td>
        <td><b>60</b></td>
    </tr>
    <tr>
        <td>Ilse Ferris</td>
        <td>Hennepin County</td>
        <td>31</td>
        <td>5</td>
        <td><b>36</b></td>
    </tr>
    <tr>
        <td>Charles Potter</td>
        <td>Anoka County</td>
        <td>33</td>
        <td>0</td>
        <td><b>33</b></td>
    </tr>
    <tr>
        <td>David Courtright</td>
        <td>St. Louis County</td>
        <td>13</td>
        <td>0</td>
        <td><b>13</b></td>
    </tr>
    <tr>
        <td>Tim Delong</td>
        <td>Stearns County</td>
        <td>10</td>
        <td>0</td>
        <td><b>10</b></td>
    </tr>
    <tr>
        <td>Casey Love</td>
        <td>Ramsey County</td>
        <td>9</td>
        <td>1</td>
        <td><b>10</b></td>
    </tr>
    <tr>
        <td>Devonne Kent</td>
        <td>Wright County</td>
        <td>9</td>
        <td>0</td>
        <td><b>9</b></td>
    </tr>
    <tr>
        <td>Melissa Fox</td>
        <td>Stearns County</td>
        <td>5</td>
        <td>0</td>
        <td><b>5</b></td>
    </tr>
    <tr>
        <td>Kelly Hiestand</td>
        <td>Wright County</td>
        <td>5</td>
        <td>0</td>
        <td><b>5</b></td>
    </tr>
    <tr>
        <td>Robert Fewins-Kalb</td>
        <td>Anoka County</td>
        <td>3</td>
        <td>0</td>
        <td><b>3</b></td>
    </tr>
    <tr>
        <td>Chris Johnson*</td>
        <td>Olmsted County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
    <tr>
        <td>Charles Clark*</td>
        <td>Hennepin County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
    <tr>
        <td>Katie Martini*</td>
        <td>Washington County</td>
        <td>1</td>
        <td>0</td>
        <td><b>1</b></td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
