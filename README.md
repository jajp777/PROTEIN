PROTEIN - PROTEct your INformation
 
.SYNOPSIS
- This PowerShell script is actively monitoring files in a repository to search for known or unknown ransomware.
- Capture creation new files, analyzing them and determining whether they are accepted or not by the corporation.
- Identify known files (whitelist), potential threats (blacklist) and unknown files for further processing.
- Logs creation action on files.
- Possibility of email alerts administrator detected anew ransomware.
- Alert via messagebox on the user's computer detected a new ransomware.
- Ability to disable the domain user affected by the ransomware, preventing access to the repository or other critical system objects
- Ability to disable the NIC on the user's computer affected by the ransomware, to block access to the network.

.REQUIREMENTS
- Run this script as administrator to control remote computers and users of the domain.

.NOTES
- Author		: Amador Pérez Trujillo
- Twitter		: @c0p3rnic
- Company		: http://www.newvisionsoftlan.com

	
.PARAMETER --install
- Set the path to folders to monitor, path and filename for storage logs and email of the adminsitrator to alert of a risk.
- Set the actions to perform when a ransomware was detected: Send an email and disable the user of the domain and disable computer's NIC for network access.

.PARAMETER --monitor
- Start monitoring the Folders... Start the Game!!!

.PARAMETER --configure
- Re-configure path of folders to monitor and storage the logs, email address and severity and actions to do after a detection.

.PARAMETER --path
- Echo by console the configuration files for checking purposing.

.PARAMETER --logs
- Echo by console the log file.

.PARAMETER --find /u:username /a:action /d:date
- Find logs by user.
    /u:username Find all logs performed by the user.
    /a:action   Find all logs group by action performed. Action = Created, Deleted, Changed, Renamed.
    /d:date     Find all logs performed in a specific date. Format dd/mm/aaaa.
