# create

The `sumocli sources create` command creates a source attached to a collector in the Sumo Logic organisation.

## Usage

Usage: `sumocli sources create [options]`

The following options are required for this command:

* `--collectorId` - Id of the collector to attach the source to.
* `--name` - Name of the source.

The following options are options for this command:

* `--category` - The sourceCategory for the source.
* `--fields` - Fields to the add to the source.
* `--httpSource` - Creates a http source.
* `--messagePerRequest` - Specifies each request to the source is a single message.
* `multilineProcessingEnabled` - Specifies that multiple lines represent a single message.