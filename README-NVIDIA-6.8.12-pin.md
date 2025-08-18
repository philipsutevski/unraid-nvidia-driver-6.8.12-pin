# Nvidia Driver plugin pinned to 6.8.12-Unraid

This variant installs the upstream plugin package and patches it to query and download driver assets from the `6.8.12-Unraid` release tag.

Install on Unraid:

1. Copy the raw URL of `nvidia-driver-6.8.12-pin.plg` hosted somewhere you control (e.g., your GitHub repo raw link), or place it on the Unraid USB under `/boot/config/plugins/`.
2. From Unraid WebUI: Plugins → Install Plugin → paste the raw URL → Install.
3. Open Settings → Nvidia Driver. The Available Versions list and downloads will be sourced from the `6.8.12-Unraid` tag.

Notes:
- This pins only the release source for asset discovery. It does not change driver selection behavior (latest, PRB, NFB, manual version) except that all queries resolve within that tag.
- To revert, uninstall this plugin and install the upstream plugin from Community Apps. 