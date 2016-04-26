PROTEIN - PROTEct your INformation
 
.SYNOPSIS
- This script is an actively monitoring for files in a repository to search for known or unknown ransomware.
- PROTEIN captures the action of creation new files, analyzing them and determining whether they are valid or not for the corporation.
- PROTEIN Identifies known files (whitelist), potential threats (blacklist) likewise unknown files for further processing.
- PROTEIN logs every creation action on files on your server.
- Possibility to email alerts to an administrator when a new ransomware is detected.
- PROTEIN alerts, via messagebox on the user's computer, when a new ransomware is detected.
- PROTEIN disables domain's user affected by the ransomware, preventing the access to the repository by the ransomware or other critical system objects.
- PROTEIN disables the NIC on the user's computer affected by the ransomware, to block the access to the network.

.REQUIREMENTS
- Run this script as an administrator to control computers and domain users remotely.

.NOTES
- Author		: Amador Pérez Trujillo
- Twitter		: @c0p3rnic
- Company		: http://www.newvisionsoftlan.com

	
.PARAMETER --install
- Set the path to folder to monitor, path and filename for storage logs and email of the adminsitrator to alert of a risk.
- IMPORTANT!!! Anti_malware_config folder MUST BE in c:\ on your File Server

.PARAMETER --monitor
- Start monitoring the Folders... Start the Game!!!

.PARAMETER --configure
- Re-configure path of folders to monitor and storage the logs, email address..

.PARAMETER --path
- Echo by console the configuration files for checking purposing.

.PARAMETER --logs
- Echo by console the log file.
