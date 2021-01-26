# get

The `sumocli roles get` command gets information about a specific role from a Sumo Logic organisation.

## Usage

Usage: `sumocli roles get [options]`

The following option is required for this command:

* `--id` - Id of the role you want to retrieve information about.

The following option is optional for this command:

* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id

