# Authentication

Sumocli uses two authentication methods;

* Environment variables 
* Credentials file

When you run a command in sumocli it will first check to see if a credentials file exists, if it can't find one then it will fall back to environment variables this is to ensure that sumocli can run in CI/CD pipelines. The sections below explain the requirements for each authentication type.

## Environment Variables

Environment variable authentication is useful when running sumocli in a CI/CD pipeline. The following environment variables need to be set to allow for proper authentication.

```text
SUMO_ACCESS_ID: abcefghi

SUMO_ACCESS_KEY: AbCeFG123

SUMO_ENDPOINT: https://api.<regioncode>.sumologic.com/api/
```

For a full list of Sumo Logic regions to API endpoints see this page: [https://help.sumologic.com/APIs/General-API-Information/Sumo-Logic-Endpoints-and-Firewall-Security](https://help.sumologic.com/APIs/General-API-Information/Sumo-Logic-Endpoints-and-Firewall-Security)

{% hint style="info" %}
When you are setting the SUMO\_ENDPOINT you need to ensure you add the trailing ' / ' at the end of the URL.
{% endhint %}

## Credentials File

The credentials file stores the same information as the environment variables however, it can be generated interactively using [sumocli login](../commands-cli/login.md). The credential file is stored in the following locations depending on your operating system.

```text
Windows: C:\Users\<username>\.sumocli\credentials\creds.json

Macos: /User/<username>/.sumocli/credentials/creds.json

Linux: /Usr/<username>/.sumocli/credentials/creds.json
```

The contents of the credential file is as follows:

```javascript
{
  "accessid": "abcefghi",
  "accesskey": "AbCeFG123",
  "endpoint": "https://api.<regioncode>.sumologic.com/api/"
}
```

