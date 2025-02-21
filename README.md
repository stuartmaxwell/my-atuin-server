# My Atuin Server

My set up notes for getting this running on Coolify.

## Server Setup

- Set up the following environment variables:

```env
ATUIN_DB_URI=postgres://user:password@hostname/database
ATUIN_HOST=0.0.0.0
ATUIN_OPEN_REGISTRATION=true
ATUIN_PORT=8888
```

- Change the Coolify domain name to: `https://custom.domain.com:8888`

## Client Setup

- Edit the `~/.config/atuin/config.toml` file.
- Set the sync_address as follows: `sync_address = "https://custom.domain.com"`
- Run the registration: `atuin register -u <YOUR_USERNAME> -e <YOUR EMAIL>`
- Save the key somewhere safe: `atuin key`
- After the registration, the `ATUIN_OPEN_REGISTRATION` setting above can be changed to `false`.
