# Privacy Policy — AI YouTube Production Studio

_Last updated: 2026-08-26_

AI YouTube Production Studio ("the tool") is a personal, self-hosted application
built and operated by a single individual (Ricardo Schroeder) for producing and
uploading videos to that individual's own YouTube channel. It is not distributed
as a service to other users.

## What data the tool accesses

When connected to YouTube, the tool requests the following OAuth scopes:

- `https://www.googleapis.com/auth/youtube.upload`
- `https://www.googleapis.com/auth/youtube.readonly`

These are used only to read basic information about the operator's own connected
channel (channel ID and title) and to upload videos, thumbnails, and metadata that
the operator produced using the tool.

The tool does not access, collect, or process data belonging to any other YouTube
user, channel, or viewer. It has no public-facing accounts, sign-up flow, or
multi-user functionality.

## How data is stored

OAuth access and refresh tokens returned by Google are written to a single JSON
file on the operator's own local machine, inside the application's private data
directory. This file:

- Is never transmitted to any third-party server.
- Is never logged, analyzed, or shared.
- Exists only on the operator's local disk, alongside the application itself.

No YouTube data, credentials, or tokens are stored in any cloud database, remote
service, or third party of any kind.

## How to revoke access

The operator can revoke the tool's access at any time in either of two ways:

1. Using the "Disconnect YouTube" action inside the application, which deletes the
   local token file immediately.
2. Directly through Google's own account permissions page at
   [myaccount.google.com/permissions](https://myaccount.google.com/permissions),
   which revokes the OAuth grant at the source regardless of the tool's local state.

## Data retention and deletion

Tokens are retained locally only for as long as the operator keeps the application
installed and connected. Deleting the local data directory, or using the
in-app disconnect action, permanently removes all stored credentials. No copy of
this data exists anywhere else.

## Contact

For questions about this policy, contact: ricardoschroeder@gmail.com
