Script btrfs-snap to automatically take btrfs snapshots daily, put them in /.btrfs/ and label with the date. Adjust the SOURCE_DIR to include absolute directory of the btrfs subvolumes to include.
If a snapshot already exists that day, it just skips that subvolume (comes in handy after adding subvolume and calling script manually).

Script btrfs-borg-backup to sync the /.btrfs/ with a borg repo for remote backup. Adjust the BORG_REPO with absolute path where borg repo is mounted, and BORG_PASSPHRASE with the passphrase for the repo.

After editing both can be added to crontab to automatically run daily.
