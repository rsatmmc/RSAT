# Download RSAT (Remote Server Administration Tools)

Download the latest version from Releases page:       
https://github.com/confyg/RSAT/releases/tag/1.412

RSAT enables IT professionals to remotely administer Windows Server roles and features from a device running Windows 10 or Windows 7 Service Pack 1.

## Introduction

RSAT can’t be installed on computers running Home or Standard editions of Windows. It is offered only for Professional or Enterprise editions of the Windows client operating system. Unless the download page explicitly states that RSAT supports a beta, preview, or another prerelease Windows version, you must use a full (RTM) operating system release to install and use it. Some users have attempted to manually circumvent the RSAT MSU restrictions to deploy it on unsupported Windows editions or builds. Doing so breaches the terms of the Windows end-user license agreement.

Installing RSAT is similar to deploying Adminpak.msi on Windows 2000 or Windows XP client machines. There is one important difference, though: on Windows 7, the tools are not available immediately after installation. You need to enable the required tools manually through Control Panel. To do so, go to **Start** > **Control Panel** > **Programs and Features**.

With RSAT packages for Windows 10, all tools are turned on by default after the package is installed. If you want to disable tools you don’t intend to use on Windows 7, open **Turn Windows features on or off**.

For Windows 7, after the RSAT package is installed, you must manually enable the tools for the roles and features you plan to manage.

If you’re managing roles or features on remote servers from Windows Server 2012 R2, you don’t need to install any additional tools. Start the Add Roles and Features Wizard on Windows Server 2012 R2 or later, then on the **Select Features** page, expand **Remote Server Administration Tools**, select the tools you require, and complete the wizard to finish the installation.

## RSAT for Windows 10, version 1809 or later versions

> **Note**
> The **Turn Windows features on and off** dialog in Control Panel isn’t available to use.

Starting with Windows 10 version 1809, installing RSAT is a bit different from earlier methods. RSAT is now included with the operating system and can be added via **Optional Features**.
