# PowerShell-Script-Practice-

## PowerShell Tutorial
[PowerShell_Tutorial](https://www.tutorialspoint.com/powershell/index.htm)

### Cmdlets
Cmdlets are way different from command in other command-shell environment in the following manner
* Cmdlets are .NET Framework class objects; and not just stand-alone executables.
* Cmdlets can be easily constructed from as few as a dozen lines of code.
* Parsing, error presentation, and output formatting are not handled by cmdlets. It is done by the Windows PowerShell runtime.
* Cmdlets process works on objects not on text stream and objects can be passed as output for pipelining.
* Cmdlets are record-based as they process a single object at a time.

### Files and Folders
1. Creating Folders
    > `New-Item -Path 'G:\code\Test Folder' -ItemType Directory`
2. Creating Files
    > `New-Item -Path 'G:\code\Test Folder\Test File.txt' -ItemType File`
3. Copying Folders
    > `Copy-Item 'G:\code\Test Folder' 'G:\code\Test Folder1'`
    > `Copy-Item 'G:\code\Test Folder' -Destination 'G:\code\Test Folder1'` (recursively)
4. Copying Files
    > `Copy-Item 'G:\code\Test Folder\Test File.txt' 'G:\code\Test Folder1\Test File1.txt'`
    > `Copy-Item -Filter *.txt -Path 'G:\code\Test Folder' -Recurse -Destination 'G:\code\Test Folder1'`
5. Deleting Folders
    >
6. Deleting Files
    >
7. Moving Folders
    >
8. Moving Files
    > 
9.  Rename Folders
    >
10. Rename Files
    >
11. Retrieving Items
    >
12. Check Folders Existence
    >
13. Check Files Existence
    >`Test-Path G:\code\Test Folder\Test File.txt`

### Dates and Timers
1. Get System Date
    >
2. Set System Date
    >
3. Get System Time
    >
4. Set System Time
    > `Test-Path D:\temp\test\test.txt`

    > `$timeToAdd = New-TimeSpan -Minutes -60`
    > `set-date -adjust $timeToAdd`