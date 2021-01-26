# create

The `sumocli azure create` command creates Azure infrastructure required to send logs or metrics to Sumo Logic. This command also creates a collector and source in Sumo Logic so there is no user intervention required.

## Usage

Usage: `sumocli azure create [options]`

The following options are required for this command:

* `--category` - sourceCategory for the source.
* `--prefix` - User defined string that is used to name Azure resources, can only contain numbers, lowercase letters and a max length of 10.

When running this command you need to specify one of the following depending on what type of data you are collecting:

* `--blob` - Used to collect logs from a storage account (useful for NSG Flow Logs).
* `--diagnostic` - Used to collect logs using Azure Diagnositcs.
* `--metrics` - Used to collect metrics using Azure Diagnositcs.

See the [Azure Authentication](authentication/azure.md) page for the different ways to authenticate.
