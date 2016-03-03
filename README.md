# mergerfs-tools
Optional tools to help manage data in a mergerfs pool

## mergerfs.fsck

Audits permissions and ownership of files and directories in a mergerfs mount and allows for manual and automatic fixing of them.

It's possible that files or directories can be duplicated across multiple drives and that their metadata become out of sync. Permissions, ownership, etc. This can cause some strange behavior depending on the mergerfs policies used. This tool helps find and fix those inconsistancies.

```
$ mergerfs.fsck -v -f manual /path/to/dir
```

## mergerfs.dedup

**TO BE CREATED**

Finds and deduplicate files and directories.

## mergerfs.rebalance

**TO BE CREATED**

Simplifies rebalancing of files across drives.

## mergerfs.mktrash

Will create [FreeDesktop.org Trash specification](https://specifications.freedesktop.org/trash-spec/trashspec-1.0.html) compatible directories on a mergerfs mount. Helps minimize issues with apps which `rename` into the trash directory.

```
$ mergerfs.mktrash /mountpoint
```
