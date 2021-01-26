# Update

The `sumocli users update` command updates a user in the Sumo Logic organisation.

## Usage

Usage: `sumocli users update [options]`

The following options are required for this command:

* `--firstName` - First name of the user.
* `--isActive` - Is the account active defaults to true.
* `--lastName` - Last name of the user.
* `--id` - Id of the user.
* `--roleIds` - Comma deliminated list of roles to assign to the user.

The following options are options for this command:

* `--merge` - Merge is set to true by default meaning only the updated required fields will be updated on the user. If it is set to false the required fields will overwrite what is set on the user.
* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id