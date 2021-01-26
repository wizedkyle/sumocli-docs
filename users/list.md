# list

The `sumocli users list` command lists users that are available in the Sumo Logic organisation.

## Usage

Usage: `sumocli users list [options]`

By default, users list will list the first 100 users that are available in the Sumo Logic organisation. The command line flags that are available for users list are all optional. The following command line flags are available:

* `--email` - Email address of the user.
* `--results` - Specify the number of results to return, 100 results are returned by default.
* `--sort` - Sort the results by firstName, lastName or email.
* `--output` - Specify the field to export the value from. The following fields can be exported:
  * name
  * description
  * filterPredicate
  * users
  * capabilities
  * id