# Upload to Paperless

A [Dropzone 5](https://aptonic.com/dropzone5/) action for uploading documents to a [Paperless-ngx](https://docs.paperless-ngx.com/) server.

Drag files onto the action to upload them to your Paperless-ngx instance. Supports any file type your Paperless server can consume (PDFs, images, Office documents, etc.).

## Installation

1. Download `Upload to Paperless.dzbundle`
2. Double-click to install in Dropzone, or copy it to `~/Library/Application Support/Dropzone/Actions/`

## Configuration

When you add the action, Dropzone will prompt you to fill in:

| Field | Value |
|-------|-------|
| **Server** | Your Paperless URL (e.g. `paperless.example.com`) |
| **Port** | Only if using a non-default port, otherwise leave blank |
| **Username** | Your Paperless username, or `api` for token auth |
| **Password** | Your Paperless password, or your API token if username is `api` |
| **Remote Path** | Leave blank (not used) |
| **Root URL** | Leave blank (not used) |

### Authentication

The action supports two authentication methods:

- **Username & Password** — uses HTTP Basic Auth
- **API Token** — enter `api` as the username and your API token as the password. You can generate a token in Paperless under My Profile.

### HTTPS / HTTP

The action defaults to `https://`. If your instance uses plain HTTP, enter the full URL including the scheme (e.g. `http://paperless.local`).

## Usage

- **Drag files** onto the action to upload them to Paperless
- **Click** the action to open your Paperless instance in the browser

Upload progress is shown in real-time, weighted by file size when uploading multiple documents.

## License

[MIT](LICENSE)
