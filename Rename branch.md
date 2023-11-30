
```
@echo OFF
title Rename Git Branch

:start
cls
Echo ===============================
Echo Git Branch Renaming Tool
Echo ===============================
Echo.

set "oldBranch="
set /P "oldBranch=Enter the old branch name: "

if "%oldBranch%"=="" (
    Echo Old branch name cannot be empty.
    pause
    goto :start
)

set "newBranch="
set /P "newBranch=Enter the new branch name: "

if "%newBranch%"=="" (
    Echo New branch name cannot be empty.
    pause
    goto :start
)

:init
Echo Old Branch: %oldBranch%
Echo New Branch: %newBranch%
Echo.

:choice
set /P "c=Are you sure you want to continue (Y/N)? "
if /I "%c%" EQU "Y" goto :renameBranch
if /I "%c%" EQU "N" goto :cancel
goto :choice

:renameBranch

rem git checkout %oldBranch%
rem git branch -m %newBranch%
git branch -m %oldBranch% %newBranch%
git push origin :%oldBranch% %newBranch%
git push origin -u %newBranch%

Echo.
Echo Branch renamed successfully.
pause
goto :start
exit

:cancel
Echo.
Echo Rename canceled!
pause
goto :start`
