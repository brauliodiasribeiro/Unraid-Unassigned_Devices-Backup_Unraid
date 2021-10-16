# Unraid-Unassigned-Bkp
This script make backup to PLUG & PLAY devices or FIXED devices and make incremental or sync backup.

<form action="https://www.paypal.com/donate" method="post" target="_top">
<input type="hidden" name="business" value="QVR5JEKFBASVW" />
<input type="hidden" name="no_recurring" value="0" />
<input type="hidden" name="currency_code" value="USD" />
<input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" border="0" name="submit" title="PayPal - The safer, easier way to pay online!" alt="Donate with PayPal button" />
<img alt="" border="0" src="https://www.paypal.com/en_BR/i/scr/pixel.gif" width="1" height="1" />
</form>

# PLUG & PLAY DEVICES
You connect the device into usb, the "Unassigned Devices Plugin" mount, make backup, and unmount.

- Incremental backup:
	- The frequency is when you plug the device into USB.

- Sync backup:
	- The frequency is defined in "Day_Sync" variable of the script.

# FIXED DEVICES
The devices are already connected but not mounted. The script mount, make backup, and unmount.

- Incremental backup:
	- You need creat a script and schedule backup frequency in "CA User Scripts -> Schedule Disabled". Example: "Schedule Daily" or "Schedule Weekly".
This schedule is from the incremental backup.

- Sync backup:
	- The frequency is defined in "Day_Sync" variable of the script.

# INCREMENTAL BAKUP
Don't delete anything from the backup directory, just copy new or modified files.

# SYNC BACKUP
Mirroring. If the file isn't in the source directory, it'll be deleted from the backup directory.
