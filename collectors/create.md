# create

The `sumocli collectors create` command creates a collector in the Sumo Logic organisation.

## Usage

Usage: `sumocli collectors create [options]`

The following option is required for this command:

* `--name` - Name of the collector.

The following options are optional for this command:

* `--category` - sourceCategory for the collector, this will overwrite the categories on configured sources.
* `--description` - Description for the collector.