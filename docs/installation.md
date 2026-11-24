# Installation

**Planned release · December 13, 2026**

## Choose the installer

Open [GitHub Releases](https://github.com/GibsonAB/robotics-ecosystem-2027/releases). When the release is available, check its notes for the Ubuntu version, CPU architecture, ROS 2 distribution, and prerequisites verified for that installer. Download the .deb from the release assets. Install ROS and any project-specific dependencies listed in the release notes or in your workspace's instructions.

## Verify and install

Open a terminal in the download directory. Replace `DOWNLOADED_FILENAME.deb` with the actual asset name.

~~~bash
sha256sum DOWNLOADED_FILENAME.deb
~~~

Compare the full result with the SHA-256 checksum in the release notes. Once it matches, install the package:

~~~bash
sudo apt install ./DOWNLOADED_FILENAME.deb
~~~

Open **Robotics Ecosystem 2027** from the application menu. See [First run](first-run.md) for the initial ROS connection and workspace setup.

## Upgrade or remove

Follow the installer instructions for the new version. Close the app before upgrading and check the release notes for any migration steps.

To identify the installed package by its Debian package name, run `dpkg-deb -f DOWNLOADED_FILENAME.deb Package` against the downloaded installer. To remove the app, pass that exact package name to `sudo apt remove`. Your ROS workspaces and recordings are separate project data. Check their locations before cleaning up any remaining app files.

See [Troubleshooting](troubleshooting.md) if the installer reports an unmet dependency or the app fails to open.
