# get

The `sumocli collectors get` command gets information about a specific collector from a Sumo Logic organisation.

## Usage

Usage: `sumocli collectors get [options]`

The following option is optional for this command:

* `--id` - Id of the collector you want to retrieve information about.
* `--name` - Name of the collector you wnat to retrieve information about.
* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id
