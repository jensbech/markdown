Set server: `bws config server-base https://vault.bitwarden.eu`.

## Set and retrieve token into local env

Set token into Keychain: `security add-generic-password -a "bws_access_token" -s "Bitwarden Secrets Manager" -w "your_access_token_here"`
Get environment variable from Keychain: `export BWS_ACCESS_TOKEN=$(security find-generic-password -a "bws_access_token" -s "Bitwarden Secrets Manager" -w)`

- `- a` = account, `- s` = name

The token should be associated with a project.

Now can run stuff and insert all environment variables into environment: `bws run --project-id 9d72d613-8d1f-4435-8676-b2c10167aa1 -- bun env.ts`
