# login

The `sumocli login` command is used to interactively provide a Sumo Logic Access Id, Access Key and API endpoint.

{% hint style="info" %}
This command is suitable only for interactive use, it will not be suitable for CI/CD pipelines. For more information on authenticating with sumocli see [Authentication](../concepts/authentication.md).
{% endhint %}

## Usage

Usage: `sumocli login`

## Credentials Storage

By default sumocli will save your Sumo Logic Access Id and Access Key in plain text in a file called creds.json. If you are generating this file using `sumocli login` you will be told where the file is going to be saved and you will have the option to cancel.

For more information about the credentials file including where they are stored on certain operating systems see the [Authentication](../concepts/authentication.md) page.

