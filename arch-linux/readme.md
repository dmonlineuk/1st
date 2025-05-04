# Scripts

Recommended approach would be to run `. pac-inst` first, then `. 1drive-inst`, and the rest in any order your like :-)

## OneDrive

For installing OneDrive:

`. 1drive-inst`

This should get, build and install everything needed to get OneDrive working. Once installed,

`onedrive -s` can be used as a one-time sync, and

`systemctl enable onedrive@dan.service` and `systemctl start onedrive@dan.service`

for using the service in systemd.

## DisplayLink

To enable support with usb-c docks display outputs:

`. displink-inst`

## AUR builds

This one covers:
- VS Code (official)
- hyprshot

`. aur-builds`

## GIT Setup

This is required to enable pushing to github, security of credentials is maintained
using `gpg` and `pass` packages, linked to the Git Credential Manager. Get set up with:

`. git-setup`

## KeePass cli

KeePass database is in OneDrive, so that should be set up first. Get the cli using:

`. kpcli-inst`

This uses lots of AUR packages so may seem 'verbose' as it builds them. I prefer to do
this instead of AUR helpers, but each to their own.

KNOWN ISSUE - as of writing there is a mistake in the sha256 verification that needs user intervention.

## Steam

Clearly optional, needs 'multilib' library enabled. Install with:

`. steam-inst`

NOTE: Look out when prompted that the correct vulkan/32bit drivers are chosen e.g. nvidia, intel or amd.

## Pacman

There is a copy of `pacman.conf` but this is really to demonstrate we need to enable multilib for Steam.
