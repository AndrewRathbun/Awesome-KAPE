# Awesome-KAPE
In line with other Awesome GitHub repos, Awesome-KAPE serves as a curated list of KAPE-related resources, including but not limited to blog posts, videos, and links to relevant GitHub repos. 

## Official KAPE Links
- [Download KAPE](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kroll-artifact-parser-extractor-kape)
- [KAPE Enterprise License](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kroll-artifact-parser-extractor-kape/enterprise-license)
  - TL;DR: if you make money off KAPE in a paid engagement, you need a license! Otherwise, it's free for everyone else including but not limited to Law Enforcement, students, researchers, etc
- [KAPE Training](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kroll-artifact-parser-extractor-kape/training)

## Tool-Related GitHub Repos

### KAPE

- [KapeFiles](https://github.com/EricZimmerman/KapeFiles) - This repository contains all the Targets and Modules utilized by KAPE to collect and process forensic artifacts
- [KapeDocs](https://github.com/EricZimmerman/KapeDocs) - This repository serves as the backend for KAPE's KapeDocs page, linked [here](https://ericzimmerman.github.io/KapeDocs/)

### EZ Tools

The command line versions of [Eric Zimmerman's Tools](https://ericzimmerman.github.io/#!index.md) ship with KAPE, so they are very relevant to KAPE's overall functionality. The following EZ Tools have KAPE Modules written for them and these repos should be monitored for activity given that they will directly influence KAPE output:

  - [AmcacheParser](https://github.com/EricZimmerman/AmcacheParser)
  - [AppCompatCacheParser](https://github.com/EricZimmerman/AppCompatCacheParser)
  - [bstrings](https://github.com/EricZimmerman/bstrings)
  - [EvtxECmd](https://github.com/EricZimmerman/evtx)
    - Namely, [Maps](https://github.com/EricZimmerman/evtx/tree/master/evtx/Maps) where EvtxECmd Maps are located
  - [JLECmd](https://github.com/EricZimmerman/JLECmd)
  - [LECmd](https://github.com/EricZimmerman/LECmd)
  - [MFTECmd](https://github.com/EricZimmerman/MFTECmd)
  - [PECmd](https://github.com/EricZimmerman/PECmd)
  - [RBCmd](https://github.com/EricZimmerman/RBCmd)
  - [RecentFileCacheParser](https://github.com/EricZimmerman/RecentFileCacheParser)
  - [RECmd](https://github.com/EricZimmerman/RECmd)
    - Namely, [BatchExamples](https://github.com/EricZimmerman/RECmd/tree/master/BatchExamples) where Batch Files are located
    - Also, [RegistryPlugins](https://github.com/EricZimmerman/RegistryPlugins) which are used by RECmd (and Registry Explorer) to generate more efficient/actionable output
  - [SQLECmd](https://github.com/EricZimmerman/SQLECmd)
    - Namely, [Maps](https://github.com/EricZimmerman/SQLECmd/tree/master/SQLMap/Maps) where SQLECmd Maps are located
  - [SrumECmd](https://github.com/EricZimmerman/Srum)
  - [SumECmd](https://github.com/EricZimmerman/Sum)
  - [WxTCmd](https://github.com/EricZimmerman/WxTCmd)

## Resources

### Blog Posts/Guides

- [AboutDFIR's KAPE Guide](https://aboutdfir.com/toolsandartifacts/windows/kape/)
- [Exploring KAPE’s Graphical User Interface in v0.8.2.0](https://www.kroll.com/en/insights/publications/cyber/exploring-kapes-graphical-user-interface)

### YouTube Videos

- [A Guide to Eric Zimmerman's command line tools (EZ Tools)](https://youtu.be/GhCZfCzn2l0)
- [Behind The Incident Eric Zimmerman](https://youtu.be/IuiIGzm7k34)
- [Child Exploitation Investigation – Express Analysis with KAPE](https://youtu.be/-Tgc28hHAhw)
- [Conducting Efficient Insider Threat Investigations using KAPE](https://youtu.be/LxjDUMk0w2g)
- [Enabling KAPE at Scale](https://youtu.be/YF-jDoh8BFM)
- [Enhancing Event Log Analysis with EvtxEcmd using KAPE](https://youtu.be/BIkyWexMF0I)
- [Episode 80: Learning about the KAPE tool.](https://youtu.be/TDpAsSnjhBw)
- [Episode 81: Understanding and Using KAPE Target Files](https://youtu.be/DdUqfktcPa4)
- [Episode 82: Understanding and Using KAPE Module Files](https://youtu.be/aT0xy0VvlSQ)
- [Episode 83: Explaining the KAPE GUI Version -Target Side](https://youtu.be/bCSrUOoDXU4)
- [Episode 84: Explaining the KAPE GUI Version - Module Side](https://youtu.be/2cK7SZjQXuY)
- [Episode 85: Running KAPE through the GUI Version](https://youtu.be/a_x0IgTW67o)
- [Episode 86: Reviewing the Output Created by KAPE](https://youtu.be/HqioWJBmeLA)
- [Episode 87: Introducing and Using Timeline Explorer](https://youtu.be/Hy8ZIc86tCo)
- [Episode 88: Comparing EZViewer to Other Free File Viewers](https://youtu.be/r4X5ONbwlSk)
- [Episode 89: Finding Forensic Badness in 3 Minutes or Less](https://youtu.be/V-pBwAGsQvw)
- [Introduction to KAPE](https://youtu.be/L9H1uj2HSb8)
- [KAPE + EZ Tools and Beyond - OSDFCon 2019 - Eric Zimmerman](https://youtu.be/ZCj7cbWwUOs)
- [Triage Collection and Timeline Analysis with KAPE](https://youtu.be/iYyWZSNBNcw)

## Unofficial Version History

| Date       | Version | Notes |  
|-|-|-|
| 2016-02-16 | 0.8.1.0 | - Add support for UNC paths for `--tsource` and `--tdest`<br> - Better detection when out of storage space on destination<br>- Add check when `--mdest` and `--tdest` are the same and disallow it<br>- Warn when `--msource` != --tdest<br>- Clarify EULA section 1.3 as it relates to usage |  
| 2019-03-05 | 0.8.2.0 | - Change ConsoleLog from being file based to memory based. ConsoleLog is saved to --tdest and/or --mdest as necessary<br>- Remove --dcl option since ConsoleLog is in memory now<br>- Added --sync switch to automatically update Targets and Modules from the KapeFiles GitHub repository<br>- Add --overwrite along with --sync to overwrite any local targets and modules<br>- In the ConsoleLog, remove extra line feeds and only show first letter of log level<br>- gkape updated to allow for editing and creating new targets and modules, including validation<br>- Added ability to specify multiple targets and modules on the command line (--target filesystem,eventlogs for example)<br>- Add Progress information to Title bar of Console or PowerShell window<br>- Gkape interface overhauled<br>- Added PowerShell script for automatic updates of the main KAPE package<br>- Add --mvars switch which allows passing in key:value pairs to modules<br>- Polish and tweaks |
| 2019-03-15 | 0.8.3.0 | - Added %kapeDirectory% variable that is replaced with the full path to where kape.exe was executed from. Useful for having a reference point for config files to pass to modules, etc.<br>- Added SFTP support. Server name, port, and username are required. See help screen for more details and switches. SFTP password, when present, will be redacted from the ConsoleLog<br>- Added zip to container options. Works like VHD(x) containers, except things just get zipped up<br>- When targeting $J, only copy the non-sparse part of the file. This makes for a much smaller (and faster!) collection<br>- Added _kape.cli support. _kape.cli should contain one or more KAPE command lines (one per line). When KAPE sees this file on start up, it executes one copy of KAPE per line in the file, then renames _kape.cli by adding a timestamp to the front of the file. See https://twitter.com/EricRZimmerman/status/1104212779299426304 for more details and example usage<br>- Remove --toe option<br>- In modules, for ExportFile property, %fileName% will get replaced using the name of the file being processed. Example: ExportFile: TeraCopy-history_%fileName%.csv |
| 2019-04-24 | 0.8.3.2 | - Truncate CopyLog filename when more than one target is used to avoid overly long file name creation<br>- Fix for rare issue when expanding wildcards in targets<br>- When using --sync, any targets or modules in !Disabled folders will be removed from the Targets or Modules directory so they stay disabled<br>- Added warning in gkape when either of the flush options are enabled. Also added a means to disable the warning in gkape<br>- Preserve last access timestamps even if last access updates are enabled.<br>- Tweak path detection so that things like '--tdest ..\destination' works, which allows for using relative paths on command line (i.e. when you do not know drive letter ahead of time)<br>- control and software updates<br>- When using --mlist and --mdetail, KAPE Will list any missing binaries along with the URL to download the missing files<br>- Updated to the most recent targets and modules |
| 2019-05-01 | 0.8.3.3 | - Updated nuget packages<br>- Fix issue copying files from VSS based on a change introduced in 0.8.3.2<br>- Handle long files paths gracefully when using container options. When a long file name is encountered, the file will be copied to a new name and the original full path/name is preserved in a text file in the <Root>\LongFileNames directory. The Copylog will still indicate original source and new destination |
| 2019-05-01 | 0.8.3.4 | - Fix for collecting from UNC paths |
| 2019-05-03 | 0.8.3.5 | - Fix for long file name issue when passing in multiple targets on the command line that caused the generated file names to become too long for containers |
| 2019-05-16 | 0.8.4.0 | - Faster VSC discovery (4x faster!) and better timestamp resolution for VSC creation<br>- Improve VSC access to allow for copying out NTFS system files ($MFT, $J, etc.) from VSCs<br>- Tweak to when a directory shows up under --tdest (right before its needed vs earlier in previous releases)<br>- Reference files pulled from VSCs using ''VSS#' vs a path under ___vssMount for consistency<br>- Updated/new targets and modules<br>- Updated EZ Tools binaries<br>- General refactoring and cleanup |
| 2019-06-04 | 0.8.4.2 | - Added --cu switch. When using batch mode (_kape.cli), allows for deleting config files when the batch run completes<br>- Added detection of CPU architecture (x86 vs x64) and a way to run x86 specific binaries for modules. See the "Modules" documentation for full details. In short, x64 support is assumed. If x86 is needed, name the binary the same as what is in the module, but end the name with '_x86'. Example: If you had Executable: foo.exe in a module, having a file named "foo_x86.exe" next to foo.exe, foo_x86.exe would be the actual program executed. Use --debug to see the selection process take place<br>- Added documentation URL to KAPE help screen and clickable hyperlink in lower left of gkape<br>- Tweak output of --tlist/--mlist to include slightly less detail so there is not as much scrollback needed. --tdetail and --mdetail include the removed information if needed<br>- Add directory KAPE runs from to console log<br>- Fix for using *relative* paths with mdest |
| 2019-06-25 | 0.8.5.0 | - Detect invalid paths (\\server\C$: or c:\temp\c: for example)<br>- Updated nuget and controls<br>- Only show informational messages when they make sense (ie copy stats of files were found, etc)<br>- Handle case where --tdest is a directory like H:\C and treating that path as root vs assuming root is H:<br>- LOWER minimum .net dependency to .net 4.5 for kape.exe and 4.5.2 for gkape.exe<br>- Updated EZ Tools binaries<br>- Added details about files being skipped to CopyLog.txt (example: Skipping 'l:\Windows\System32\config\RegBack\SAM' with SHA-1 'DA39A3EE5E6B4B0D3255BFEF95601890AFD80709' as a file with same hash has already been copied) |
| 2019-07-01 | 0.8.5.1 | - Add %m to gkape interface<br>- Handle spaces in Target and Module names in gkape. It is recommended to not have spaces in names, but gkape now properly adds quotes around target and module switches if any of the selected items contains spaces<br>- Remove dependency for deduplication on whether 'Process VSCs' is checked in gkape.<br>- nuget and control updates<br>- Updated EZ Tools binaries |
| 2019-07-22 | 0.8.5.2 | - Redirect and capture standard error stream in console apps when --debug is used. Prior to this, only standard out stream was showing up in the console log<br>- Add dedicated log tracking skipped files (deduplicated and excluded).  It is a CSV ending with 'skiplog.csv'. Thanks to Troy Larson for the idea!<br>- Add SHA-1 exclusion via --hex. Takes a text file containing one SHA-1 per line. Any files with the same SHA-1 as an entry in the file is skipped (and logged in 'skiplog.csv')<br> |
| 2019-07-29 | 0.8.5.3 | - gkape tweak for new SHA-1 option moving around<br>- Fix issue with --zip container option when writing to UNC path<br>- Allow blank SFTP password<br>- Digitally sign Get-KAPEUpdate.ps1 script |
| 2019-08-09 | 0.8.6.2 | - When using transfer options, transfer module output to destination when --zm true is used. This pushes the output from modules as a zip file to the destination server. You can still optionally transfer target collection too<br>- For batch mode, add --ul switch. This stands for "Use linear" and when set on an entry (it should be the first one ideally), KAPE will run each instance from _kape.cli one at a time, vs spawning all at once. Useful for fine grained control over batch mode<br>- In gkape, remember selected targets and modules in gkape when viewing config via double click. This makes it possible to examine configurations and not have to reselect everything previously selected<br>- Change --mvars separator to ^ since comma was often used in variable definitions. Also tweaked how variables containing : are treated (they just work now vs. being truncated)<br>- When KAPE updates a module's output file to avoid overwriting an existing file, report the name of the new output file to the Console so its possible to know which input file corresponds to which output file<br>- Fix rare issue with module processing when standard out and standard error get written to concurrently<br>- Change redirecting StandardError to output file in modules to writing it to the Console. This prevents programs that mix normal output on StdErr from messing up output files<br>- Added 'Append' property (optional) to Module's processor section. If true, data is appended to the value for ExportFile. If append is false, a new, unique filename is generated to prevent files from being overwritten<br>- Standardize all timestamps used in log files, file names, etc. to correspond to same timestamp (when KAPE was executed) vs when files get created. this makes it easier to group related things together<br>- Added AWS S3 transfer support via --s3* switches<br>- Added Azure Storage transfer (SAS Uri) via --asu switch<br>- Updated gkape for newest features |
| 2019-08-15 | 0.8.6.3  | - Fix in gkape for mvars building (update separator to ^ vs old value of ,)<br>- Replace %m (Machine name) and %d (timestamp) in --zip, --vhx, and --vhdx switches. You can even do both at once to get a timestamped file with machine name<br>- Other minor tweaks and nuget updates |
| 2019-08-26 | 0.8.7.0 | - Refactored --sync command to allow for and respect subdirectories in Targets and Modules. --sync will reorganize things based on the KapeFile repo. Configs not in KapeFiles repo end up under !Local directory<br>- Overhauled Targets and modules organization. Compound targets and modules DO NOT need to be updated to new locations. KAPE will locate the base configs as needed on the fly<br>- With the new config organization, KAPE can now pull all configs under a directory specified in --target or --module. In this way, directories act like a compound config<br>- tlist and mlist now expect a path to look for configs. Use . to start. All configs in the provided path are displayed as well as subdirectories<br>- Added Folder column in gkape in Targets and Modules grids. Grouping by this column makes it easy to see what is in various folders<br>- Tweaks to transfer setting validation to ensure destination is writable<br>- Removed --sow switch<br>- When in SFTP server mode, display the KAPE switches needed to connect to the SFTP server for each defined user. This makes it as easy as copy/paste to tell KAPE to push to SFTP server<br>- Add --sftpu switch, which defaults to TRUE, that determines whether to display SFTP server user passwords when in SFTP server mode<br>- Added FollowReparsePoint and FollowSymbolicLinks to Target definition. These are optional and should be used on an as needed basis. The default for both is false if they are not present. This is the behavior KAPE has always had up to this point. Setting to true will follow the reparse or sym link which some programs use (Box, OneDrive, etc)<br>- Other minor tweaks and nuget updates |
| 2019-09-07 | 0.8.7.1 | - Detect of any FTK processes are running, warn, and exit unless new --ifw switch is also set. This warns people to not use FTK Imager to mount images which can lead to problems.<br>- Added check for new version of KAPE at end of run if Internet connectivity exists. If a new version is present, the new version number available is shown along with a message about how to update.<br>- Fix issue with empty directory paths being too long for containers in some cases<br>- Other tweaks for various edge cases |
| 2019-09-18 | 0.8.7.2 | - Swapped out SFTP client with more robust implementation<br>- Added logging of file upload and download initiation to SFTP mode. Now both the start of and completion of the upload is shown<br>- Added logging of file deletion to SFTP mode<br>- gkape GUI tweaks<br>- When syncing, a unique GUID is added to any config names that end up in !Local so the file names are unique. This prevents the warning about duplicate config names<br>- Other --sync tweaks |
| 2019-09-26 | 0.8.7.3 | - sftp transfer tweaks (use large buffers to send data, add transfer speed to Title bar)<br>- Updated zipping component (~35% faster zipping!)<br>- Updated SFTP config format (be sure to read the docs and check out the example) |
| 2019-10-23 | 0.8.8.0 | - Remove target information from container names and log files<br>- Delete SkipLog file if it is empty at end of run<br>- Fix issue with not finding files in VSCs due to symlink processing changes<br>- Cleaned up other names of log files<br>- Updated controls and nuget packages |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
