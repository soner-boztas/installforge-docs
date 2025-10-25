# Code-Signing Setup Packages

## Introduction

Code signing is an essential security and trust mechanism in modern software distribution. It ensures that your setup
packages are **authentic, untampered and issued by a verified publisher**.
When your setup package is code-signed, users can confidently install your software without worrying about potential
tampering or malware injection.

## Why Code Signing Matters

### **Authenticity and Trust**

When you sign your setup package with a valid code signing certificate, your identity as a software publisher is
verified by a trusted certificate authority (CA).  
This allows users (and Windows itself) to verify that the software truly comes from you, rather than from an unknown or
malicious source.

### **Integrity Protection**

A digital signature ensures that the setup package has not been modified after signing.  
If any byte of the file changes — for example, through corruption or tampering — Windows will detect the mismatch and
display a warning to the user.

### **Improved User Experience**

Unsigned installers often trigger warning dialogs such as:

> *“Windows protected your PC”*  
> *“The publisher could not be verified”*

By code-signing your setup package, these warnings are replaced by a clear identification of your company name and a
smoother installation flow, resulting in greater user confidence and higher installation success rates.

### **Compliance with Security Policies**

Many corporate IT environments and antivirus solutions block unsigned executables by default. Code-signing ensures
your setup packages comply with organizational and security requirements, making them deployable in
professional environments.

### **SmartScreen Reputation**

For Windows, code-signed applications can build up a **SmartScreen reputation** over time.  
Unsigned installers, by contrast, are more likely to trigger SmartScreen warnings, potentially discouraging users from
running your software.

## Code-Signing InstallForge Setup Packages

InstallForge allows you to code-sign your setup packages during the build process by integrating with *Sign Tool* from
*Microsoft*.

The following executables will be signed during the build process:

* Setup package executable
* Uninstaller executable
* Updater (Visual Update) executable (if packaged)

### Prerequisites

InstallForge internally relies on *Sign Tool* from *Microsoft* to code-sign setup packages during the build process. 
That means, that *Sign Tool* must be available on your system in order to code-sign setup packages with InstallForge.

!!! info

    More information about *Sign Tool* and its installation can be found in the
    [Microsoft docs](https://learn.microsoft.com/en-us/dotnet/framework/tools/signtool-exe).

### Configuring Code-Signing in InstallForge

In order to code-sign setup packages with InstallForge, follow these steps:

1. In the InstallForge IBE, navigate to the `Build` section on the [Left Pane].
2. In the [Main Pane], locate the `Code Signing` subsection.
3. Activate `Sign setup package executable` by checking the corresponding checkbox.
4. Provide the command-line that will be passed to *Sign Tool* (`signtool.exe`) during the build process.

[Main Pane]: ../getting-started/quick-start-guide.md#overview-of-the-ibe-interface
[Left Pane]: ../getting-started/quick-start-guide.md#overview-of-the-ibe-interface
