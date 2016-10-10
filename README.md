# Variants

The Variants project provides an import package and sample data to demonstrate an implementation of Variant Configuration.

> Note: Variants are targeted to be addressed in a future release of Aras Innovator. Please see the [Aras Public Roadmap for more information](http://www.aras.com/plm-roadmap/?keyword=IR-033578).

## Project Details

**Built Using:** Aras 11.0 SP7
**Browsers Tested:** Internet Explorer 11, Firefox 38 ESR, Chrome

> Though built and tested using Aras 11.0 SP7, this project should function in older releases of Aras 11.0 and Aras 10.0.

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed (version 11.0 SPx preferred)
2. Aras Package Import tool
3. Variants import package

### Install Steps

1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
  * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
  * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\Variants\Import\imports.mf` file in the Manifest File field.
6. Select **Variants** in the Available for Import field.
7. Select Type = **Merge** and Mode = **Thorough Mode**.
8. Click **Import** in the top left corner.
9. Close the Aras Package Import tool.
10. Optional: Import the sample data.
  * Open up AML Studio or Nash (http://<server name>/<web alias>/Client/scripts/nash.aspx)
  * Enter your admin credentials and login.
  * Copy the contents of `..\Data\VariantsSampleData.xml` and paste into AML Studio/Nash.
  * Execute the AML.

You are now ready to login to Aras and try out Variants.

## Usage

1. Log in to Aras as admin.
2. Navigate to **Design > Parts** in the table of contents (TOC).
3. Search for Part with part number "VArmrest" and open for viewing.
4. Click the Variants tab to view variations of the VArmrest Part.

> Note: The project also adds "Option Codes" and "Option Constraints" under the Portfolio category in the TOC. These are used to define and configure variants.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

For more information on contributing to this project, another Aras Labs project, or any Aras Community project, shoot us an email at araslabs@aras.com.

## Credits

Original Aras community project written by Peter Schroer at Aras Corp.

Project rewritten for Aras 11.0 by Rob McAveney.

Documented and published by Eli Donahue at Aras Labs. @elijdonahue

## License

Aras Labs projects are published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.
