[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate?business=QVR5JEKFBASVW&no_recurring=0&currency_code=USD)
## Description
* This script make incremental or sync backup to PLUG & PLAY devices or FIXED devices.

* It's possible to schedule how often and what type of the backup will be done.

* When the backup start, you'll be notified by the email. When it finishes, too.

## Incremental Backup
* Don't delete anything from the backup directory, just copy new or modified files.

* Plug & Play: Just plug the device into USB.

* Fixed: They are already connected but not is mounted.
	 - Schedule the execution frequency in "CA User Scripts -> Schedule Disabled".
	 - Example: "Schedule Daily" or "Schedule Weekly".

## Sync Backup
* Mirroring. If the file isn't in the source directory, it'll be deleted from the backup directory.

* Plug & Play: How often to backup is defined in the script.
	- Example: sync backup every 30 days from the last backup.

* Fixed: How often to backup is defined in the script.
	- Example: sync backup every 30 days from the last backup.

## Instructions
* Configure the variables in "script".

* Run the "script" on each device for the first time.

* A script will be created in "CA User Scripts / Script_Name"
	- (Unraid -> Settings -> User Scripts -> Script_Name").

* The folder and all device files will be created in "Src_Flash / Script_Name / Device Name"
	- (/boot/config/plugins/user.scripts/scripts/Script_Name/Device Name") and a copy in "Script_Dir / Script_Name / Device Name".

* Add the path of the folders you want to backup in "Script_Dir / Script_Name / Device Name / PATHS.txt".

* Run the "script" on each device again to sync all files and start the backup.
