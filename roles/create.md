# create

The `sumocli roles create` command creates a role in the Sumo Logic organisation.

## Usage

Usage: `sumocli roles create [options]`

The following options are required for this command:

* `--name` - Name of the role.

The following options are optionial for this command:

* `--autofill` - Automatically append all missing capability requirements. This is set to true by default. 
* `--capabilities` - Comma deliminated list of capabilities. Information about capabilities can be found here: https://help.sumologic.com/Manage/Users-and-Roles/Manage-Roles/05-Role-Capabilities.
* `--description` - Description for the role.
* `--filter` - Filter predicate for the role.
* `--users` - List of user IDs to assign to the role.
* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id