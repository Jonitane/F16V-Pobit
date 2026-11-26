# F16V-PoBit

Public downloads and update channel for the F16V-PoBit installer.

[Download the complete F16V-PoBit 2.93.2 package](https://github.com/Jonitane/F16V-PoBit-Downloads/releases/download/v2.93.2/POBIT_F16V-V2.93.2.zip)

For **2.9, 2.91, 2.92, 2.93 and 2.93.1**, enable **Updates**. Accept installer 2.4.0 first, then accept the component updates after it restarts. The installer compares each local component version with the shared catalog and downloads the modules your edition needs. The public edition changes to **2.93.2** when the required components are present. [2.93.2 release notes](https://github.com/Jonitane/F16V-Pobit/releases/tag/v2.93.2).

For a fresh installation or an edition earlier than 2.9, use the [2.93.2 complete package](https://github.com/Jonitane/F16V-PoBit-Downloads/releases/download/v2.93.2/POBIT_F16V-V2.93.2.zip), and open the included installer. Earlier clients may receive the installer update on the shared channel.

Click **Select path** and choose your aircraft path once. The installer identifies the entry and saves the setup automatically. Select Core and the optional components you want, then install them.

Keep **Updates** checked to check this repository when the installer opens. When updates are available, choose the items to download. Existing selected components are removed and installed automatically; the installer restarts itself when updating its own software. Failed replacements restore the previous files.

The path panel retains its title, instructions, target status and **Guide**. Its only selection action is **Select path**. The header contains only the **Updates** checkbox.

Directory rules remain configurable through `F16V-PoBit.exe --set-layout path-to-rules.json`; the command migrates existing component, download and backup folders and keeps original-backup references. See the included User Guide.

This repository is a download channel. Current installers use [updates-v2.json](updates-v2.json). The [legacy feed](updates.json) serves older installers. Software-only releases do not include Core or DLC assets. Component releases are added after their normal review and delivery process; new or disabled components are never silently enabled by an update.

The release channel uses the [update-list format](update-format.json). Each component keeps its own identity and version, and each download points to a ZIP attached to a release in this repository.

Installer versions, public mod release numbers, Core versions and DLC versions are independent. The updater compares each item's own identity/version, checks its required installer version, then checks the downloaded package identity and version. GitHub release tags never substitute for a package version. When software and component updates are selected together, the installer updates first and automatically resumes only the approved component selection after restarting.

Installer caches, installation records, transaction snapshots and diagnostics are stored under the installer directory. Old game-folder management data is migrated after verification. Unreferenced failed caches are removed. Backups retain first replaced game originals only; old software, component and update payload history is discarded after the transaction completes.
