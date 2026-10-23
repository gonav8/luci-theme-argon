# Argon V2 for OpenWrt 25.12.x

This branch adds a clean Aurora-inspired interface to the Argon theme fork: responsive horizontal LuCI navigation, soft dashboard cards, calmer tables and controls, and dark-mode-aware colors. Existing Argon behavior and LuCI/plugin data remain unchanged.

The Cellular menu is supplied by the MU300 firmware's own LuCI modem/cellular packages. Install those packages on the router; Argon V2 will display their native menu and pages with the V2 styling. A theme cannot invent or fetch cellular metrics from a device plugin that is not installed.

Build with the OpenWrt 25.12.x SDK for your router architecture. See [ARGON_V2.md](ARGON_V2.md) for notes.
