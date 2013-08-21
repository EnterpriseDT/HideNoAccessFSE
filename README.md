HideNoAccessFSE
===============

CompleteFTP File-System Extension that hides from listings folder for which the user has no access.  
This extension only applies to non-Windows users and only works with CompleteFTP Enterprise Edition.

Instructions
============

* Install CompleteFTP Enterprise Edition
* Download this repository
* Use Visual Studio or Visual Studio Express to build the assembly, HideNoAccessFSE.dll
* Open CompleteFTP Manager
* Click on the Extensions tab
* Click Add extension
* Enter the following fields:
  - Name: HideNoAccessFSE
  - Type: File System
  - Assembly Path: full path of DLL
  - Adapter Class: HideNoAccessFSE.HideNoAccessFSE
  - Editor Class: EnterpriseDT.Net.FtpServer.FileSystem.Windows.FolderAdapterEditor
  - Configuration: leave blank
* Click on the Folder Types tab
* Click Add folder-type
* Enter the following fields:
  - Name: Hide-no-access Folder
  - Extension: HideNoAccessFSE
  - Allow sub-folders?: check
  - Visible: check
* Click apply

