---
hide:
  - navigation
---
# Release Notes

## Version 1.6.1 (2025-12-23)

* **Improvements for setup packages created with InstallForge:**

    * `Enhancement` Header image (which is displayed on the top right of setup wizard dialogs) now scales correctly on high-DPI displays

* **Improvements for the InstallForge builder environment:**

    * `Feature` Restored new header image available for setup packages (`super-modern` --> `images\Header_3.png`)
    * `Fix` UI glitches have been fixed [[#29]](https://github.com/soner-boztas/installforge/issues/29)
    * `Fix` Importing legacy InstallForge project files is working correctly again [[#28]](https://github.com/soner-boztas/installforge/issues/28)
    * `Other` Added toolbar button linking to the InstallForge GitHub page
  
* **Improvements for Visual Update:**
    * `Enhancement` Updated Visual Update to version `1.3.1` (see [https://docs.visualupdate.net/release-notes/](https://docs.visualupdate.net/release-notes/) for 
      details)

## Version 1.6.0 (2025-12-14)

* **Improvements for setup packages created with InstallForge:**

    * `Feature` Support for Windows Server 2025
    * `Feature` Support for `<Temp>` path constant
    * `Enhancement` Mitigated risk of false positive detections by different anti-malware applications

* **Improvements for the InstallForge builder environment:**
    
    * `Enhancement` Full CLI builder support in the InstallForge IBE GUI
    * `Enhancement` Added context menus for the Files, `Variables`, `Commands`, `License`, `Serial Validation`, `Registry` & `Shortcuts` sections
    * `Enhancement` Added notice regarding SignTool CLI arguments in order to avoid confusion
    * `Fix` Explorer bar (left pane) items are now displayed correctly with different DPI scaling settings
    * `Fix` Wrong error messages in the build log have been fixed

## Version 1.5.0 (2025-10-25)

!!! danger "Important"

    As of version `1.5.0`, the bundled version of Visual Update Express is no longer allowed to be used in a commercial 
    context. If you want to use Visual Update in a commercial context, please purchase a Pro license.
    More information can be found at [https://docs.visualupdate.net/license/](https://docs.visualupdate.net/license/).

* **Improvements for setup packages created with InstallForge:**

    * `Enhancement` Increased extraction performance during installation
    * `Enhancement` Added new setup icon and header image (`super-modern`)
    * `Enhancement` Added Korean language file (provided by user wincmd)
    * `Enhancement` Added Finish language file (provided by user jussihi)
    * `Enhancement` Added Norwegian language file (provided by user [JustablockCode](https://github.com/JustablockCode)) [[PR#2]](https://github.com/soner-boztas/installforge-translations/pull/2)
    * `Enhancement` Added Vietnamese language file (provided by user [lphucdo](https://github.com/lphucdo)) [[PR#5]](https://github.com/soner-boztas/installforge-translations/pull/5)
    * `Enhancement` Added Slovak language file (provided by user [L-Catman](https://github.com/L-Catman) from LUnetStudio) [[PR#3]](https://github.com/soner-boztas/installforge-translations/pull/3)
    * `Enhancement` Added Bahasa Malaysia language file (provided by user [fbakhda](https://github.com/fbakhda) from :simple-intel: Intel) [[PR#4]](https://github.com/soner-boztas/installforge-translations/pull/4)
    * `Enhancement` Added traditional Chinese language file (provided by user [machichima](https://github.com/machichima) from unionai) [[PR#7]](https://github.com/soner-boztas/installforge-translations/pull/7)
    * `Enhancement` Added Português Portugal file (provided by user [sacrus](https://github.com/sacrus)) [[PR#8]](https://github.com/soner-boztas/installforge-translations/pull/8)
    * `Fix` Simplified Chinese file (provided by user [DiscreteTom](https://github.com/DiscreteTom)) [[PR#9]](https://github.com/soner-boztas/installforge-translations/pull/9)

* **Improvements for the InstallForge builder environment:**
    
    * `Feature` Added new CLI builder for building setup packages within a Continuous Deployment (CD)
      pipeline
    * `Feature` Added support for automatically code-signing setup executables (setup, uninstaller and updater) 
      during the build process
    * `Enhancement` InstallForge project files are now stored in XML format. The old format is still supported for 
      backward compatibility (see `File` --> `Import` in the main menu).
    * `Enhancement` Increased build performance
    * `Enhancement` Changed default URIs for Visual Update to `https` protocol
    * `Enhancement` Updated executable resource library (`reseditx86.dll`) (built with latest VC++ compiler) for 
      enhanced stability and security
    * `Fix` Possible Invalid Memory Access (IMA) when building setup packages
    * `Fix` Fixed old URIs in the help menu
 
* **Improvements for Visual Update:**
    * `Enhancement` Updated Visual Update to version `1.3.0` (see [https://docs.visualupdate.net/release-notes/](https://docs.visualupdate.net/release-notes/) for 
      details)

## Version 1.4.4 (2023-07-18)

* **Improvements for the InstallForge builder environment:**
    * `Enhancement` Order of custom commands can be altered
    * `Enhancement` InstallForge project files can be opened via drag-and-drop
    * `Enhancement` Added tooltips for various input widgets in order to increase user experience
    * `Enhancement` Git commit hash is displayed on the `About InstallForge` dialog window

* **Other:**
    * `Enhancement` InstallForge binary application files are code-signed

## Version 1.4.3 (2023-06-16)
* **Improvements for setup packages created with InstallForge:**

     * `Feature` Official support for Windows 11
     * `Feature` Official support for Windows Server 2022
     * `Feature` Official support for Windows Server 2019
     * `Enhancement` Added Hebrew language file
     * `Enhancement` Added Indonesian language file
     * `Enhancement` Added Japanese language file
     * `Enhancement` Added Swedish language file
     * `Enhancement` Updated Ukraine language file 
     * `Fix` Fixed bug preventing path constant `<ProgramFilesX64>` from being resolved
     * `Fix` Fixed bug the splash screen from being displayed when configured
  
* **Improvements for the InstallForge builder environment:**
    * `Fix` Fixed bug leading to possible `Could not update all setup version information!` log message issued by 
      the IBE

## Version 1.4.2 (2020-06-17)
* **Improvements for setup packages created with InstallForge:**

     * `Enhancement` Added Romanian language file (by Chris K.)
     * `Fix` Fixed false positive issues with different anti-malware applications

* **Improvements for the InstallForge builder environment:**

    * `Feature` Added an automatic check routine for available updates
    * `Enhancement` Updated some of the user interface icons
    * `Fix` Fixed bug leading to a wrong working directory after updating InstallForge

* **Improved Visual Update Express version :**

    * `Fix` Fixed false positive issues with different anti-malware applications

## Version 1.4.1 (2020-05-10)
* **Improvements for setup packages created with InstallForge:**

    * `Feature` Support for shortcut keys
    * `Enhancement` Improved native setup engine with support for the Deflate, bzip2 and BriefLZ compression algorithms
    * `Enhancement` Updated French language file (thanks to user [slegros](https://installforge.net/forums/viewtopic.php?f=7&t=718) from the InstallForge community)
    * `Enhancement` Updated English language file
    * `Enhancement` Updated German language file
    * `Fix` Fixed a display error in the user interface (installation progress dialog)

* **Improvements for the InstallForge builder environment:**

    * `Fix` Fixed a display error of the toolbar on high DPI screens
    * `Fix` Fixed the automatic redirection of the `Default Installation Path` on the `Files` tab (when the default installation path is `<ProgramFiles>\<Company>\<AppName>\` and no company name is given, InstallForge will use `<ProgramFiles>\<AppName>\` instead)
    * `Fix` Fixed automatic redirection of the default path for startmenu shortcuts (same behaviour as for the `Default Installation Path`)

* **Improved Visual Update Express version :**
    * `Feature` Support for a new command: `ShellExecute`
    * `Enhancement` Several improvements for the update engine with better error handling and increased robustness
    * `Enhancement` The update engine now detects the [BOM] of the updatescript.ini file automatically (either no [BOM] or [UTF-8] [BOM] is valid)
    * `Enhancement` The dialog can now be minimized
    * `Enhancement` Improved `DownloadFile` command: The second parameter can now contain an optional file name which will be used for the downloaded file
    * `Enhancement` Improved `DeleteFiles` command: read-only files are also deleted
    * `Enhancement` Improved `DeleteDirectory` command: read-only files are also deleted
    * `Fix` Fixed several UI issues due to DPI Awareness

## Version 1.4 (2020-04-24)
* **Extensive improvements for setup packages created with InstallForge:**

    * `Feature` Support for custom setup executable icons
    * `Feature` [Progress bar on taskbar](https://docs.microsoft.com/en-us/windows/win32/uxguide/winenv-taskbar) is now supported for Windows versions newer than Windows 7
    * `Feature` Support for custom setup executable manifest files
    * `Feature` Support for custom setup executable icons
    * `Enhancement` Completely **new native setup engine** with several enhancements and support for the [LZMA](https://en.wikipedia.org/wiki/Lempel%E2%80%93Ziv%E2%80%93Markov_chain_algorithm) compression algorithm without any limitation regarding the size of setup files
    * `Enhancement` [DPI aware](https://docs.microsoft.com/en-us/windows/win32/hidpi/high-dpi-desktop-application-development-on-windows) graphical user interface
    * `Enhancement` Changes in the GUI
    * `Enhancement` Full [Unicode] support for setup files
    * `Enhancement` Added additional path constants
    * `Enhancement` Setup constants are now case-insensitive
    * `Enhancement` Added fast verification of setup files ([cyclic redundancy check](https://en.wikipedia.org/wiki/Cyclic_redundancy_check))
    * `Enhancement` Updated language files
    * `Enhancement` Custom variable names are now case-insensitive
    * `Enhancement` Custom variables are now initialized with a preceding _[_ and an appending _]_ character
    * `Enhancement` Extended splash screen feature (support for PNG files, alpha-channel support and fade effect)
    * `Enhancement` Icon displayed on the language selection dialog is now extracted from the setup executable icon (first found)
    * `Enhancement` Extended browse folder dialog window with new capabilities, including: resizeable window, support for drag-and-drop, reordering, button to create a new folder and a context menu.
    * `Enhancement` Improved reboot function (the `ExitWindowsEx` WinAPI call is now passing `SHTDN_REASON_MAJOR_APPLICATION` | `SHTDN_REASON_MINOR_INSTALLATION` | `SHTDN_REASON_FLAG_PLANNED` to the `dwReason` parameter, see also [here](https://docs.microsoft.com/de-de/windows/win32/shutdown/system-shutdown-reason-codes))
    * `Other` Removed support for custom dynamic link Libraries

    * **Improvements for the uninstaller**

        * `Feature` Support for [progress bar on taskbar](https://docs.microsoft.com/en-us/windows/win32/uxguide/winenv-taskbar)
        * `Feature` Display icon shown in [Apps and Features](https://support.microsoft.com/en-us/help/4028054/windows-10-repair-or-remove-programs) can now be changed
        * `Enhancement` Improved native uninstaller engine
        * `Enhancement` Uninstaller configuration files are now created in JSON format
        * `Enhancement` Icon of uninstaller is now modifiable
        * `Enhancement` Information for estimated installation size and date are provided for [Apps and Features](https://support.microsoft.com/en-us/help/4028054/windows-10-repair-or-remove-programs), resp. the [uninstaller key](https://learn.microsoft.com/en-us/windows/win32/msi/uninstall-registry-key?redirectedfrom=MSDN)
        * `Enhancement` Display icon shown in [Apps and Features](https://support.microsoft.com/en-us/help/4028054/windows-10-repair-or-remove-programs) can now be changed
        * `Enhancement` Icon displayed on the uninstaller dialog is now extracted from the uninstaller executable icon (first found)

* **Improved InstallForge builder environment**
    * `Feature` Added PNG support for wizard and header image
    * `Feature` Drag and drop support for the file manager
    * `Enhancement` Improved GUI ([DPI aware](https://docs.microsoft.com/en-us/windows/win32/hidpi/high-dpi-desktop-application-development-on-windows))
    * `Enhancement` Full [Unicode] support
    * `Enhancement` Improved product serial manager supporting custom masks
    * `Enhancement` Improved license editor
    * `Enhancement` Improved builder log widget
    * `Enhancement` The IBE main window can now be minimized when building a setup package
    * `Enhancement` The IBE now automatically adds specific [version information](https://docs.microsoft.com/en-us/windows/win32/menurc/versioninfo-resource?redirectedfrom=MSDN) to setup package executables using [rcedit](https://github.com/electron/rcedit) from GitHub
    * `Enhancement` Value name in `Add Registry Value` dialog  is now optional (for default registry value)
    * `Enhancement` Added PNG support for wizard and header image
  
* **Improved Visual Update Express version**
    * `Feature` Support for secure connections (https)
    * `Enhancement` [DPI aware](https://docs.microsoft.com/en-us/windows/win32/hidpi/high-dpi-desktop-application-development-on-windows) GUI
    * `Enhancement` Full [Unicode] support (also for [Unicode] characters within the update script file)
    * `Enhancement` Improved icon (16×16 px icon now has a higher quality; also added a 24×24 px icon)

## Version 1.3.2.1 (2017-08-17)
* `Fix` Fixed bug in the Visual Update Express module

## Version 1.3.2 (2016-09-11)
* `Fix` Fixed “Setup Error -f” bug due to a [Unicode] issue within the setup engine

## Version 1.3.1 (2016-05-11)
* `Enhancement` Improved setup engine making setups less vulnerable to changes in setup executable’s resource files

## Version 1.3 (2016-03-29)
* `Feature` InstallForge setups now display the installation progress on the taskbar (only on Windows versions newer than Windows Vista)
* `Feature` Added option allowing users to disable the os-version check routine
* `Feature` Added check routine for InstallForge project files of different versions
* `Feature` Shortcut icons can be altered as of now
* `Feature` Command line arguments can be passed when starting programs after finishing setups
* `Enhancement` Support for Windows 10 and Window Server 2016
* `Enhancement` When adding registry entries or variables, the value name field can be left empty
* `Enhancement` Changed format of project files (content of project files is in pure [ASCII] format as of now)
* `Enhancement` Integrated web help in InstallForge environment
* `Fix` Fixed bug when loading project files with license texts
* `Fix` Fixed possible crash when compiling projects with license texts
* `Fix` GUI fixes within the IBE
* `Other` Removed “Import Language..” from InstallForge environment menu

## Version 1.2.9.2 (2014-04-10)
* `Enhancement` Added Chinese (Simplified) language file (thanks to user _JBob_)
* `Enhancement` Added Dutch language file (thanks to user _walt61_)
* `Enhancement` Added Greek language file (thanks to _JoyFoundry LTD_)
* `Enhancement` Added Hungarian language file (thanks to _Pál L._)
* `Fix` Fixed issue when checking for Windows 8.1

## Version 1.2.9 (2014-04-10)
* `Feature` Added support for custom commands
* `Enhancement` Improved IBE
* `Fix` Fixed -f setup error

## Version 1.2.8 (2014-04-08)
* `Enhancement` Compatibility with Windows 8.1
* `Enhancement` Integration of the newest version of _Visual Update Express_
* `Enhancement` Removed MSVCR100 dependency
* `Enhancement` Fixed possible crash when building setups

## Version 1.2.7 (2012-11-03)
* `Feature` _Visual Update Express_ integration
* `Enhancement` Compatibility with Windows 8
* `Enhancement` Improved setup engine
* `Enhancement` New icon for the uninstallation module

## Version 1.2.6.2 (2011-01-28)
* `Feature` Registry entries can be removed optionally
* `Feature` Default value of a registry key can be set

## Version 1.2.5 (2010-10-18)
* `Fix` Fixed bug in setup engine occurring on Windows Server 2003

## Version 1.2.4 (2010-08-07)
* `Enhancement` Improved uninstaller engine

## Version 1.2.3 (2010-06-01)
* `Feature` Added support for custom variables
* `Feature` Added support for command-line parameters for shortcuts
* `Feature` Name of the uninstaller file is alterable
* `Enhancement` Improved uninstaller engine
* `Fix` Fixed bug when displaying the name of the file currently being installed

## Version 1.2.2 (2010-05-06)
* `Enhancement` Setups request for admin mode
* `Enhancement` Resumed online update service
* `Fix` Fixed crash bug in the IBE

## Version 1.2.1 (2009-04-29)
* `Enhancement` Windows 7 compatibility

## Version 1.2 (2008-07-01)
* `Feature` Added option allowing setups to create shortcuts for all users
* `Feature` Compression methods for setup packages can be changed
* `Feature` Added support for environment variables for setup packages
* `Enhancement` Optimized setup engine
* `Enhancement` Changed order of setup dialogs

## Version 1.1 (2007-11-13)
* `Enhancement` Modifications in the GUI
* `Fix` Bug fixes

## Version 1.0.3 (2007-10-13)
* `Enhancement` Updated FSU (online update module)

## Version 1.0.2 (2007-10-10)
* `Enhancement` Added new language files (French by _GG_, Italian by _oridan_, Portuguese by _Rex_)

## Version 1.0.1 (2007-08-11)
* `Enhancement` Added new images for the setup wizard dialog

## Version 1.0 (2007-08-02)
* `Feature` Multi-language support for online-updater
* `Enhancement` Updated language files
* `Fix` Fixed bugs in the setup engine and IBE

## Version 0.9 (2007-07-17)
* `Enhancement` Windows Vista support
* `Enhancement` Updated language files

## Version 0.8 (2007-05-20)
* `Fix` Bugs in FSU (online update module) have been fixed
* `Fix` Bug fixes in the setup engine

## Version 0.7.1 (2007-05-04)
* `Enhancement` GUI changes in setup wizard
* `Enhancement` Updated language files
* `Fix` Several bug fixes in the setup engine

## Version 0.7 (2007-05-02)
* `Feature` Setup packages display the size of files to be installed as of now
* `Enhancement` GUI changes in setup wizard

## Version 0.6 (2007-05-01)
* `Fix` Fixed rendering issue for rebar control

## Version 0.5 (2007-04-30)
* `Feature` Implemented online update feature (FSU)
* `Fix` Bug fixes

## Version 0.4 (2007-04-29)
* `Feature` Implemented splash-screen feature
* `Fix` Bug fixes

## Version 0.3 (2007-04-28)
* `Feature` Implemented serial-check feature
* `Fix` Bug fixes

## Version 0.2 (2007-03-27)
* `Fix` Bug fixes

## Version 0.1 (2007-03-15)
* Initial release

[ASCII]: https://en.wikipedia.org/wiki/ASCII
[BOM]: https://en.wikipedia.org/wiki/Byte_order_mark
[Unicode]: https://en.wikipedia.org/wiki/Unicode
[UTF-8]: https://en.wikipedia.org/wiki/UTF-8
