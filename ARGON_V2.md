# Argon V2 (OpenWrt 25.12.x)

Argon V2 is an Aurora-inspired visual refresh of this Argon fork. It adds a compact, responsive top navigation, cleaner light/dark surfaces, tighter information hierarchy, and unified card, table, button, and status styling. It does not replace LuCI or alter the data and controls supplied by router packages.

## MU300 / Cellular menu

The Cellular menu and its pages are owned by the MU300 firmware's LuCI applications (for example, modem/cellular management packages), not by a theme. Argon V2 preserves LuCI's generated menu tree and styles any installed cellular/modem page in the same dashboard visual language. Install the MU300 cellular packages separately; their menu items will appear automatically when registered by LuCI.

## Build

Use the OpenWrt 25.12.x SDK for the target architecture, include this repository as `package/luci-theme-argon`, select `luci-theme-argon`, and compile with the SDK's normal package build command. The package version is `2.5.0-1`.
