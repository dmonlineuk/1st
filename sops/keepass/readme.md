# KeePass

General instructions to using my KeePass database in linux

## kpcli

Other tools exist, but kpcli is simple and encourages more cli use.
Relies heavily on aur, a `kpcli-inst` script exists to build itself and 
ensure all dependencies are present.

## Database location

Important - this is stored in my OneDrive, so that must be set up
first. Once sync'd, here is where it should be found:

`~/OneDrive/kpdb/Database.kdbx`

## Automated DB access

For simplicity, an alias `kpd` will be used, should be added to `.bashrc`

However, for obvious security reasons, no password will be saved to
this repo, but use of an excluded `--pwfile` can make things easier if 
preferred.


