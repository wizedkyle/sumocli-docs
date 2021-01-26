# list

The `sumocli collectors list` command lists collectors that are in the Sumo Logic organisation.

## Usage

Usage: `sumocli collectors list [options]`

* `--filter` - Name of a role that exists in the Sumo Logic tenancy.
* `--limit` - Maximum number of results returned.
* `--offline` - Lists offline collectors, set to false by default.
* `--offset` - Offset into the list of colectors.
* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id