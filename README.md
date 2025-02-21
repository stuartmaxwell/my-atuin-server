# my-atuin-server
My Atuin Server

## Server Setup

Set up the following environment variables:

```env
ATUIN_DB_URI=postgres://user:password@hostname/database
ATUIN_HOST=0.0.0.0
ATUIN_OPEN_REGISTRATION=true
ATUIN_PORT=8888
```

## Client Setup

- Edit the `~/.config/atuin/config.toml` file.
- Set the sync_address as follows: `sync_address = "https://custom.domain.com"`
- After the registration, the `ATUIN_OPEN_REGISTRATION` setting above can be changed to `false`.
