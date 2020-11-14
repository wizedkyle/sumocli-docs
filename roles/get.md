# get

The `sumocli roles get` command gets information about a specific role from a Sumo Logic organisation.

## Usage

Usage: `sumocli roles get [options]`

By default, roles list will list the first 100 roles that are available in the Sumo Logic organisation. The command line flags that are available for roles list are all optional. The following command line flags are available:

* `--id` - Id of the role you want to retrieve information about.
* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id

