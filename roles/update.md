# update

The `sumocli roles update` command updates a role in the Sumo Logic organisation.

## Usage

Usage: `sumocli roles update [options]`

The following options are required for this command:

* `--capabilities` - Comma deliminated list of capabilities. Information about capabilities can be found here: https://help.sumologic.com/Manage/Users-and-Roles/Manage-Roles/05-Role-Capabilities
* `--description` - Description for the role
* `--filter` - Filter predicate for the role
* `--id` - Id of the role
* `--name` - Name of the role
* `--users` - List of user IDs to assign to the role

The following options are options for this command:

* `--autofil` - Automatically append all missing capability requirements. This is set to true by default. 
* `--merge` - Merge is set to true by default meaning only the updated required fields will be updated on the role. If it is set to false the required fields will overwrite what is set on the role.
* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id