# Unraid-Unassigned-Bkp

This script make backup to PLUG & PLAY devices or FIXED devices and make incremental or sync backup.
#
# PLUG & PLAY DEVICES
# You connect the device into usb, the "Unassigned Devices Plugin" mount, make backup, and unmount.
# Incremental backup:
# 	The frequency is when you plug the device into USB.
# Sync backup:
# 	The frequency is defined in "Day_Sync" variable of the script.
#
# FIXED DEVICES
# The devices are already connected but not mounted. The script mount, make backup, and unmount.
# Incremental backup:
# 	You need creat a script and schedule backup frequency in "CA User Scripts -> Schedule Disabled". Example: "Schedule Daily" or "Schedule Weekly".
#	This schedule is from the incremental backup.
# Sync backup:
# 	The frequency is defined in "Day_Sync" variable of the script.
#
# INCREMENTAL BAKUP: Don't delete anything from the backup directory, just copy new or modified files.
#
# SYNC BACKUP: Mirroring. If the file isn't in the source directory, it'll be deleted from the backup directory.
