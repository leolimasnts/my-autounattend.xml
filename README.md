# Windows Installation & Cleanup `autounattend.xml`

This `autounattend.xml` file was generated using [https://schneegans.de/windows/unattend-generator/](https://schneegans.de/windows/unattend-generator/).

This repository contains an `autounattend.xml` file designed to automate and streamline the Windows installation process, focusing on removing pre-installed applications (bloatware), disabling certain features, and allowing for interactive computer name input for a cleaner, more efficient operating system.

## Features

This `autounattend.xml` configuration performs the following key actions:

* **Bypasses Installation Requirements**: Skips checks for TPM, Secure Boot, and RAM during installation.

* **Automates OOBE (Out-Of-Box Experience)**: Bypasses network requirements and hides the EULA page during OOBE.

* **Interactive Computer Name**: Prompts the user to enter a computer name during the setup process.

* **Removes Pre-installed Applications**: Uninstalls a wide range of default Windows applications and capabilities, including:

    * 3D Viewer

    * Bing Search

    * Clipchamp

    * Copilot

    * Cortana

    * Dev Home

    * Family Safety

    * Feedback Hub

    * Get Help

    * Internet Explorer

    * Mail and Calendar

    * Maps

    * News

    * Notepad (Classic)

    * Office 365

    * OneDrive

    * OneNote

    * OpenSSH Client

    * Outlook

    * Paint 3D

    * People

    * Power Automate Desktop

    * Quick Assist

    * Skype

    * Solitaire Collection

    * Steps Recorder

    * Sticky Notes

    * Teams

    * Get Started

    * To Do

    * Voice Recorder

    * WordPad

    * Xbox Apps

    * Your Phone

    * Zune Music

    * Zune Video

* **Disables Specific Features**:

    * Turns off Windows Copilot.

    * Disables automatic chat installation.

    * Disables various content delivery and app suggestion features.

    * Disables Widgets.

    * Disables Game DVR app capture.

* **Configures System Settings**:

    * Sets the time zone to `E. South America Standard Time`.

    * Configures password expiration to unlimited.

    * Enables long paths.

    * Sets PowerShell execution policy to `RemoteSigned`.

    * Disables last access timestamp updates.

    * Removes default Start Menu pins.

    * Disables Windows Consumer Features.

## Usage

To use this `autounattend.xml` file during a Windows installation:

1.  **Download**: Download the `autounattend.xml` file from this repository.

2.  **Prepare Installation Media**: Copy the `autounattend.xml` file to the root directory of your Windows installation media (USB drive or ISO).

    * **Important**: The file *must* be named `autounattend.xml` and placed in the root of the installation media.

3.  **Start Installation**: Boot your computer from the prepared Windows installation media.

4.  **Automated Process**: The Windows setup will automatically detect and use the `autounattend.xml` file to apply the specified configurations. You will be prompted to enter a computer name during the process.

## Important Notes & Disclaimer

* **Review Before Use**: It is highly recommended to review the contents of the `autounattend.xml` file before using it to ensure it aligns with your specific needs and preferences. Modifying system settings and removing components can have unintended consequences.

* **Use at Your Own Risk**: This file modifies core Windows components and settings. Use it at your own risk. The creator is not responsible for any data loss or system instability that may arise from its use.

* **Compatibility**: This file is configured for `amd64` architecture and specific language/locale settings (`en-US` UI, `pt-BR` system/user locale). Adjust these settings if your requirements differ.

## Customization

You can customize this `autounattend.xml` file by importing it into the [unattend-generator website](https://schneegans.de/windows/unattend-generator/) and editing the settings there. After making your desired changes, you can export the updated XML file.

Always test any modifications in a virtual machine or non-critical environment before applying them to a production system.
