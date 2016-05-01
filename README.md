## ABOUT ##
Git: unix-user-group-auditor
Purpose: To analyse local group membership of users on a unix server. Useful when performing an audit work and confined to a windows PC and Powershell
Required: /etc/group and /etc/passwd file
Output: Outputs a CSV file with the following tags username, password, user_id, group_id, user_id_info, home_dir, shell, primary_group, secondary_group
Author: Sam Granger

## EXECUTION POLICY ##
To run open powershell as an Administrator and run 'Set-ExecutionPolicy Bypass'

## USAGE ##
Usage  : unixUserGroupsAudit.ps1
           -passwdFile file-name-of-passwd-file
           -groupFile file-name-of-group-file
           -serverName name-of-server-files-came-from
           [-outputPath output-path]

Example: unixUserGroupsAudit.ps1 -passwdFile ".\passwd" -groupFile ".\groupFile" -serverName "server123"