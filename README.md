# F16V-PoBit

Public downloads and update channel for the F16V-PoBit installer.

[Download the installer](https://github.com/Jonitane/F16V-Pobit/releases/latest)

Click **Select path** and choose your aircraft path once. The installer identifies the entry and saves the setup automatically. Select Core and the optional components you want, then install them.

Keep **Updates** checked to check this repository when the installer opens. When updates are available, choose the items to download. Existing selected components are removed and installed automatically; the installer restarts itself when updating its own software. Failed replacements restore the previous files.

The path panel retains its title, instructions, target status and **Guide**. Its only selection action is **Select path**. The header contains only the **Updates** checkbox.

Directory rules remain configurable through `F16V-PoBit.exe --set-layout path-to-rules.json`; the command migrates existing component, download and backup folders and keeps original-backup references. See the included User Guide.

This repository is a download channel. Updates are listed in [updates.json](updates.json). Software-only releases do not include Core or DLC assets. Component releases are added after their normal review and delivery process; new or disabled components are never silently enabled by an update.

The release channel uses the [update-list format](update-format.json). Each component keeps its own identity and version, and each download points to a ZIP attached to a release in this repository.

Installer versions, public mod release numbers, Core versions and DLC versions are independent. The updater compares each item's own identity/version, checks its required installer version, then checks the downloaded package identity and version. GitHub release tags never substitute for a package version. When software and component updates are selected together, the installer updates first and automatically resumes only the approved component selection after restarting.
