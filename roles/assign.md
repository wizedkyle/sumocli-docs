# assign

The `sumocli roles assign` command assigns a role to a user in the Sumo Logic organisation.

## Usage

Usage: `sumocli roles assign [options]`

* `--roleId` - Id of the role you want to assign to the user.
* `--userId` - Id of the user you want to assign to the role.
* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id