# dotNetTips.Dev.Utility.App

Below is info for this app from dotNetTips.com. To install go to: http://bit.ly/dotNetTipsDevApp

## Clean Visual Studio & SQL Server Temp and Cached Files
This feature will quickly remove temporary and cached files created by Visual Studio and SQL Server. The reason I created this app is because from time to time Visual Studio builds will error for some unexplained reason, especially after getting new source from source control. It’s because these temporary and cached files that are not removed by Visual Studio and can cause these types of issues. After just one day of coding this app can find and delete thousands of files!

This feature will automatically detect where these files are and delete them as long as they are not in use and the user has proper permissions. To help remove some of these issues, the app will stop IIS, SQL Server and other services before deleting files and then restart them after it’s done.

### Features
- Auto detects temporary and cache folders created by Visual Studio and SQL Server
- Fast! Can delete up to 2K files per second!
- Starts and stops Windows services that could prevent files from being cleaned.

## Quickly Backup Source Code
This feature will quickly backup your Visual Studio code files. I use this feature to backup source files before retrieving source from source control (since some of these programs wipe out code changes) and at the end of the day.

When the first backup is triggered and then every 7 days (default), this feature will scan all of your drives for source code. For every folder found, it will ask you if you want to add that folder to the backup process. There is even a "turbo backup" that will backup files with the archive flag set.

This feature will backup files to your OneDrive folder so they will be in the cloud (location can be changed via the config file). By default, this feature will remove any backup folders older than 7 days.

## Features Coming In The Next Version
- Properly chooses OneDrive folder by default to backkup files to. It favors a OneDrive business account over a personal account.
