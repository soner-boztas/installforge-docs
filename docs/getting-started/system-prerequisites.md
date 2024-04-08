# System Prerequisites

This section lists the system prerequisites for operating InstallForge. A distinction is made here between the
IBE (_InstallForge Builder Environment_), that is used to create setup packages, and the setup packages (including the
uninstaller) themselves.

The following definitions should be noted in this context:

`Build System`

:   System on which the IBE is operated on in order to build setup packages.

`Target System`

:   System which is targeted by the setup packages built using the IBE.

Before using InstallForge, please make sure that the requirements listed are met by the system(s)
being operated.

=== "Build System Prerequisites"

    | Category           | Prerequisite                                                               |
    |--------------------|----------------------------------------------------------------------------|
    | Operating System   | :simple-windowsxp: Windows 7 or later                                      |
    | CPU                | :simple-intel: :simple-amd: Any Intel or AMD CPU based on x86 architecture |
    | RAM                | 1 GB                                                                       |
    | Disk Space         | 10 MB                                                                      |
    | Monitor Resolution | 1024 x 768 px                                                              |

=== "Target System Prerequisites"
    
    | Category           | Prerequisites                                                              |
    |--------------------|----------------------------------------------------------------------------|
    | Operating System   | :simple-windowsxp: Windows 7 or later                                      |
    | CPU                | :simple-intel: :simple-amd: Any Intel or AMD CPU based on x86 architecture |
    | RAM                | 128 MB                                                                     |
    | Disk Space         | N/A (depends on the size of target files packaged)                         |
    | Monitor Resolution | 1024 x 768 px                                                              |

!!! note

    Please note that despite "Windows 7 or later" being stated in the target system prerequisites, setup packages 
    can technically target Windows 2000, Windows XP, Windows Server 2003, Windows Vista and Windows Server 2008 as 
    well. However, these operating system are not officially supported.
