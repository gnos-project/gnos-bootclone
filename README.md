# GNOS bootclone

Manage ZFS bootable clones

## Usage

```
NAME: bootclone
DESC: Bootable ZFS root clones manager
AUTH: elias@gnos.in

USAGE:
  list               Detail bootable clones
  create NAME [SRC]  Create clone, SRC supports @snapshot
  delete [-s] NAME   Delete clone and origin
  detach [-s] NAME   Detach clone from origin
  update             Update managed grub.cfg
  help               Help
```

`-s` option also destroys the origin snapshot.

## Install

Specific ZFS layout creation is done by GNOS Core [installer](https://github.com/gnos-project/gnos-gnowledge).
