# dod_dtp

Software to enable requirements of AR 600-85.

From AR 600-85:

## 4–20. Drug-Testing Program software 
All Army units are required to use the DOD-developed Drug Testing Computer Program as their predominant method for selecting Soldiers for random testing and preparing the required testing forms and labels. Units should submit at least 95 percent of their urinalysis specimens using the DOD DTP software.

- DOD DTP Software
- Current Unit Roster (Excel document with columns: 'First Name', 'Last Name', EDIPI, Rank, 'Unit Assigned')

Overall design of the software:

## Drug-Testing Program
The DOD DTP is software designed to manage and automate a unit-level substance abuse program. The UPL uses the software to maintain a list of personnel in the unit, randomly select Soldiers for drug testing, and print required forms and bottle labels. CSPs may also use the DOD DTP for managing civilian drug testing.

### Generate a unit roster (with Name, EDIPI, Unit Assigned)

1. Visit [DTMS](https://dtms.army.mil/DTMS/Default.aspx)
2. Select "Reporting" > "Report Center" > "Report List"
3. Select the "Unit" tab and the "Unit ACFT Roster Report"

Direct Link to export report (Requires DTMS Access)

- [Unit ACFT Roster Report](https://dtms.army.mil/DTMS/ReportCenter/DisplayReport?type=DTMS.Modules.Army.Reports.Mvc.Reports.ACFTClassUnitRoster%2C%20DTMS.Modules.Army.Reports.Mvc%2C%20Version%3D1.0.0.15%2C%20Culture%3Dneutral%2C%20PublicKeyToken%3Dnull)

4. Generate the report and export the information to Excel.

### Load the unit roster into dod_dtp and then generate a UA list

5. Load the file into dod_dtp. 
6. Generate a percentage based list of Soliders to take the UA.
7. The labels for bottles may be generated from the tool.
8. Export the list of Soldiers that took the UA and when they took the UA. 

## Printed Documents:
- Personnel to be Tested (Notification Copy)
- Personnel to be Tested (Work Copy)
- Urinalysis Register
- DD Form 2624 (Front and Back)
- Bottle Label

Use Avery 5163 Labels to print the bottle labels.


