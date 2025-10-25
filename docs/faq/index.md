---
hide:
  - navigation
  - toc
---

# Frequently Asked Questions

??? question "Are there any costs associated with using InstallForge?"

    No! InstallForge is free to use. An exception applies only if you want to use Visual Update for commercial purposes.
    In this case, you must acquire a valid Visual Update Pro license. You can find more information about the Visual
    Update use terms in the [Visual Update License](https://docs.visualupdate.net/license).

??? question "Do setup packages created with InstallForge depend on any runtime environment (such as .NET)?"

    No, not at all! Setup packages created with InstallForge have only minimal dependencies on the Win 32 API and are 
    compatible even with old Windows versions.

??? question "Are setup packages compiled native machine code?"

    Yes! The program code of InstallForge setup package executables is pure C code compiled with
    [gcc](https://gcc.gnu.org/).

??? question "Can I deploy any application with setup packages built using InstallForge, regardless of the technology used?"

    Yes, indeed. You can deploy any application, regardless of the programming language and technology used for 
    its development, with setup packages built via InstallForge.

??? question "What is the preferred support channel for InstallForge?"

    The first place you should go is our [online forums](https://installforge.net/forums/). There are other 
    InstallForge users around who will be happy to help you with your questions and problems.

??? question "Are setup packages using the serial verification feature of InstallForge safe?"

    The answer to this question depends on how we define "safe." If we define " safe" to mean that the end-user can 
    only install your application by entering a valid serial string, the answer is "no". This is because a skilled 
    technical specialist will be able to manually extract the application packaged with your setup. However, this 
    statement also applies to all competing setup creator products. It is technically not possible to guarantee 
    absolute safety here. Nevertheless, the serial check function in InstallForge is not pointless because of that. 
    You just have to make sure that your application is activated based on the entered serial string after 
    the installation (e.g. via an online service).
