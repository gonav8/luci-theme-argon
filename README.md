# luci-theme-argon (Modified)

Argon is a clean and tidy LuCI theme. This modified version includes the **Full Internet Detector Status** feature.

## Features
- **Full Internet Detector Status**: Displays Internet, VPN, and Public IP details on the **Status/Overview** page.
- **Configurable**: Toggle the display in the Argon Config app.
- **OpenWrt 25.12 Ready**: Built using the native APKv3 format.

## Installation (OpenWrt 25.12.2)

Use `uclient-fetch` (standard in OpenWrt) to avoid issues with different `wget` versions.

```bash
# Update package list
apk update

# Install the modified Argon theme
uclient-fetch -O luci-theme-argon-2.4.3-r0.apk https://github.com/gonav8/luci-theme-argon/releases/download/v2.4.3-mod/luci-theme-argon-2.4.3-r0.apk
apk add --allow-untrusted --force-reinstall ./luci-theme-argon-2.4.3-r0.apk

# Install the modified Argon config app
uclient-fetch -O luci-app-argon-config-1.0-r0.apk https://github.com/gonav8/luci-app-argon-config/releases/download/v1.0-mod/luci-app-argon-config-1.0-r0.apk
apk add --allow-untrusted --force-reinstall ./luci-app-argon-config-1.0-r0.apk
```

## Screenshots
![Internet Detector](Screenshots/internet_detector_status.png)
