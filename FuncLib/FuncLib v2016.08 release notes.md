Functions Library release v2016.08
===
This release is the first release of the BlueZone Scripts FuncLib with combined MAXIS and PRISM functions. For this process, the PRISM functions have simply been copied over into the library. Details on individual functions are included below.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
New functions
===
**change_client_name_to_FML**
This function changes the format of a participant name. For example, "Levesseur, Wendy K" becomes "Wendy K LeVesseur."

Parameters:
* `client_name` - The name in [last], [first] [middle initial] format

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**clear_line_of_text**
Clears a field of text from the mainframe screen.

Parameters:
* `row` - the row to begin clearing
* `start_column` - the column to start clearing from

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**create_mainframe_friendly_date**
Creates a date in a way that's friendly for mainframe use, and inserts it into the screen.

Parameters:
* `date_variable` - the date to enter onto the screen
* `screen_row` - the row to enter it
* `screen_col` - the column to enter it
* `year_type`- the type of year ("YY" vs "YYYY")

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**date_converter_PALC_PAPL**
Converts a date for use on PALC or PAPL.

Parameters:
* `date_variable` - the date to convert

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**enter_PRISM_case_number**
Adds a PRISM case number into a specified row or column.

Parameters:
* `case_number_variable` - the case number to be entered (should always be `PRISM_case_number`)
* `row` - the row to enter into PRISM
* `col` - the column to enter into PRISM

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**fix_case_for_name**
Applies `fix_case` logic, but customized for names such as hyphenated surnames.

Parameters:
* `name_variable`

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**fix_read_data**
Removes underscores and excess spaces from read information, then applies the `fix_case` function to set the case correctly.

Parameters:
* `search_string` - The search string to look for

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**PRISM_case_number_finder**
Searches for the PRISM case number.

Parameters:
* `variable_for_PRISM_case_number` - the `PRISM_case_number` variable (always use this one as it's a standard)

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**PRISM_case_number_validation**
Validates that a manually entered PRISM case number is correct (13 characters, with ten digits, a dash, and two digits at the end). Outputs true or false, which can be used to force dialogs to confirm the PRISM case number is correct.

Parameters:
* `case_number_to_validate`- the `PRISM_case_number` variable (always use this one as it's a standard)
* `outcome` - outputs either `true` or `false` depending on how the function validates the number

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**select_cso_caseload**
This code is helpful for bulk scripts. This function is used to select the caseload by the 8 digit worker ID code entered in the dialog.

Parameters:
* `ButtonPressed` - The `ButtonPressed` variable used by dialogs everywhere
* `cso_id` - the CSO ID to find cases from
* `cso_name` - The CSO's name (appears in the dialog)

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**send_dord_doc**
This function requires a recipient (the recipient code from the DORD screen), and the document code (also from the DORD screen). This function adds the document. Some user involvement (resolving required labels, hard-copy printing) may be required.

Parameters:
* `recipient` - The recipient to search for
* `dord_doc`- The document you're trying to add

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**word_doc_open**
Opens a Word document and establishes needed objects for it.

Parameters:
* `doc_location` - The location of the Word document to be opened
* `objWord` - The object to be used to represent Word itself
* `objDoc` - The object to be used to represent the document itself

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**word_doc_update_field**
Updates a field in a Word form.

Parameters:
* `field_name` - The bookmark to use from your Word doc
* `variable_for_field` - The variable to write to the Word doc
* `objDoc` - The object to be used to represent the document itself

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**write_bullet_and_variable_in_CAAD**
Adds a bullet, a label, and a variable into a CAAD note. This will look like `* TEXT FROM THE BULLET: TEXT FROM THE VARIABLE`.

Parameters:
* `bullet` - The text you want before the colon in your bullet list
* `variable` - The variable or text you want after the colon in your bullet list

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**write_variable_in_CAAD**
Adds a line of text to a CAAD note.

Parameters:
* `variable` - The variable or text you want in your CAAD note

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

**write_variable_in_DORD**
Adds a line of text to a DORD doc.

Parameters:
* `string_to_write` - The variable or text you want in your DORD doc
* `recipient` - The person who will receive the DORD doc

*Merged by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Updates to existing functions
===
**add_JOBS_to_variable**
Added functionality into function to include reading the GRH PIC information. *Completed by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #272.*

**run_from_GitHub**
The error MsgBox has been updated to remove Veronica's name explicitly. *Completed by Veronica Cary (@theVKC, DHS). Resolves issue #274.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Functions depreciated in this release
===

* `memb_navigation_next` (replaced with `MAXIS_dialog_navigation`)
* `memb_navigation_prev` (replaced with `MAXIS_dialog_navigation`)
* `navigation_buttons` (replaced with `MAXIS_dialog_navigation`)
* `panel_navigation_next` (replaced with `MAXIS_dialog_navigation`)
* `panel_navigaton_prev` (replaced with `MAXIS_dialog_navigation`)
* `stat_navigation` (replaced with `MAXIS_dialog_navigation`)
* `script_end_procedure_wsh` (not replaced as it's not used anywhere)
* `step_through_handling` (not replaced as it's not used anywhere)

*Functions depreciated by Ilse Ferris (@IlseFerris, Hennepin County). Resolves issue #269.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
Other updates
===
**county_name = ""**
This constant has been modified to not work if PRISM scripts are invoked. This is done so that functionality used in PRISM to hide certain scripts at the county level can be retained. *Completed by Veronica Cary (@theVKC, DHS). Addresses issue #271.*

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
===
### Contribution statistics (07/24/2016 to 08/21/2016)

<table>
    <tr>
        <th>Scriptwriter Name</th>
        <th>Agency</th>
        <th>Commits (FuncLib)</th>
    </tr>
    <tr>
        <td><b>Veronica Cary</b></td>
        <td>DHS</td>
        <td>4</td>
    </tr>
    <tr>
        <td><b>Charles Potter</b></td>
        <td>DHS</td>
        <td>3</td>
    </tr>
    <tr>
        <td><b>Ilse Ferris</b></td>
        <td>Hennepin County</td>
        <td>2</td>
    </tr>
</table>

<i>* New scriptwriters this release</i>
