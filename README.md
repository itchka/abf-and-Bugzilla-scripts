# abf-and-Buzilla-scripts
Repo for scripts to massage abf and Bugzilla data into spreadsheets.
The scripts in this repo can be used to create a spreasheet suitable for publishing on Google Docs. It's input is the faied_mass_build_list.txt from the mass build report page.
The output can be processed by quote_fields_and_add_nl.sh which generate a specific format fo the Google sheet.
The main script is called failed_build_sheet_with_case.sh and is invoked as "failed_build_sheet_with_case.sh failed_builds_list.txt" the output file is failed_mass_rebuilds.txt.

These scripts are very crude, slow and longwinded and definately capable of improvement.. see awk.switch for ideas. Ultimately though they do produce useful output!!

Possible improvements:-
After a mass build the failed_builds_list becomes obsolete very quickly as packages are fixed. If the scripts checked for lated builds of the same packages the information from these 
could be included instead of the out of date info from the original build. If a later build was sucessful then the package could be  maked as fixed in the sheet.



Bugzilla
An additional script in this repo can be used to clean up Bugzilla's csv files for use in Google sheets.


