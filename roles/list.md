# list

The `sumocli roles list` command lists roles that are available in the Sumo Logic organisation.

## Usage

Usage: `sumocli roles list [options]`

By default, roles list will list the first 100 roles that are available in the Sumo Logic organisation. The command line flags that are available for roles list are all optional. The following command line flags are available:

* `--filter` - Name of a role that exists in the Sumo Logic tenancy
* `--results` - Specify the number of results to return, 100 results are returned by default
* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id



