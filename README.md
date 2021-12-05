[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate?business=QVR5JEKFBASVW&no_recurring=0&currency_code=USD)
# INCREMENTAL OR SYNC BACKUP TO UNRAID UNASSIGNED DEVICES
	This script make incremental or sync backup to PLUG & PLAY devices or FIXED devices.

	It's possible to schedule how often and what type of the backup will be done.

	When the backup start, you'll be notified by the email. When it finishes, too.

# INCREMENTAL BACKUP
	Don't delete anything from the backup directory, just copy new or modified files.
	
	Plug & Play: 	Just plug the device into USB.
	
 	Fixed:		They are already connected but not is mounted.
 			Schedule the execution frequency in "CA User Scripts -> Schedule Disabled".

# SYNC BACKUP
	Mirroring. If the file isn't in the source directory, it'll be deleted from the backup directory.
	
	Plug & Play:	How often to backup is defined in the script (Day_Sync).
			Example: make sync backup every 30 days from the last backup.
	
	Fixed:		How often to backup is defined in the script (Day_Sync).
			Example: make sync backup every 30 days from the last backup.
