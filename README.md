<!-- markdownlint-configure-file {
  "MD013": {
    "code_blocks": false,
    "tables": false,
    "line_length":200
  },
  "MD033": false,
  "MD041": false
} -->

[license]: /LICENSE
[license-badge]: https://img.shields.io/github/license/jerrykuku/luci-theme-argon?style=flat-square&a=1
[prs]: https://github.com/jerrykuku/luci-theme-argon/pulls
[prs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square
[issues]: https://github.com/jerrykuku/luci-theme-argon/issues/new
[issues-badge]: https://img.shields.io/badge/Issues-welcome-brightgreen.svg?style=flat-square
[release]: https://github.com/jerrykuku/luci-theme-argon/releases
[release-badge]: https://img.shields.io/github/v/release/jerrykuku/luci-theme-argon?style=flat-square
[download]: https://github.com/jerrykuku/luci-theme-argon/releases
[download-badge]: https://img.shields.io/github/downloads/jerrykuku/luci-theme-argon/total?style=flat-square
[contact]: https://t.me/jerryk6
[contact-badge]: https://img.shields.io/badge/Contact-telegram-blue?style=flat-square
[en-us-link]: /README.md
[zh-cn-link]: /README_ZH.md
[en-us-release-log]: /RELEASE.md
[zh-cn-release-log]: /RELEASE_ZH.md
[config-link]: https://github.com/jerrykuku/luci-app-argon-config/releases
[lede]: https://github.com/coolsnowwolf/lede
[official]: https://github.com/openwrt/openwrt
[immortalwrt]: https://github.com/immortalwrt/immortalwrt

<div align="center">
<img src="https://raw.githubusercontent.com/jerrykuku/staff/master/argon_title4.svg">

# A brand new OpenWrt LuCI theme (Modified)

Argon is **a clean and tidy OpenWrt LuCI theme** that allows<br/>
users to customize their login interface with images or videos.  
It also supports automatic and manual switching between light and dark modes.

**Modified version: Includes full Internet Detector status on Status/Overview.**

[![license][license-badge]][license]
[![prs][prs-badge]][prs]
[![issues][issues-badge]][issues]
[![release][release-badge]][release]
[![download][download-badge]][download]
[![contact][contact-badge]][contact]

**English** |
[简体中文][zh-cn-link]

[Key Features](#key-features) •
[Branch](#branch-introduction) •
[Version History](#version-history) •
[Getting started](#getting-started) •
[Screenshots](#screenshots) •
[Contributors](#contributors) •
[Credits](#credits)

<img src="https://raw.githubusercontent.com/jerrykuku/staff/master/argon2.gif">
</div>

## Key Features

- Clean Layout.
- Adapted to mobile display.
- Customizable theme colors.
- Support for using Bing images as login background.
- Support for custom uploading of images or videos as login background.
- Automatically switch between light and dark modes with the system, and can also be set to a fixed mode.
- **New: Full Internet Detector status display on Status/Overview page.**
- Settings plugin with extensions [luci-app-argon-config][config-link]

## Branch Introduction

There are currently two main branches that are adapted to different versions of the **OpenWrt** source code.  
The table below will provide a detailed introduction:

| Branch | Version | Description                        | Matching source                                           |
| ------ | ------- | ---------------------------------- | --------------------------------------------------------- |
| master | v2.x.x  | Support the latest version of LuCI | [Official OpenWrt][official] • [ImmortalWrt][immortalwrt] |
| 18.06 (deprecated) | v1.x.x  | Support the 18.06 version of LuCI   | [Lean's LEDE][lede]                                         |

## Getting started

### Install for OpenWrt 25.12.2 (using APK)

For the latest OpenWrt versions using the APK package manager:

```bash
# Update package list
apk update

# Install dependencies
apk add luci-compat

# Download and install the modified Argon theme
wget --no-check-certificate -O luci-theme-argon_2.4.3_all.apk https://github.com/gonav8/luci-theme-argon/releases/download/v2.4.3-mod/luci-theme-argon_2.4.3_all.apk
apk add --allow-untrusted ./luci-theme-argon_2.4.3_all.apk

# Download and install the modified Argon config app
wget --no-check-certificate -O luci-app-argon-config_1.0_all.apk https://github.com/gonav8/luci-app-argon-config/releases/download/v1.0-mod/luci-app-argon-config_1.0_all.apk
apk add --allow-untrusted ./luci-app-argon-config_1.0_all.apk
```

### Build for OpenWrt official SnapShots and ImmortalWrt

```bash
cd openwrt/package
git clone https://github.com/gonav8/luci-theme-argon.git
make menuconfig #choose LUCI->Theme->Luci-theme-argon
make -j1 V=s
```

## Notice

- Chrome browser is highly recommended. There are some new css3 features used in this theme, currently only Chrome has the best compatibility.
- Microsoft has officially retired Internet Explorer, RIP IE🙏<del>Currently, the mainline version of the IE series has bugs that need to be addressed.</del>
- FireFox does not enable the backdrop-filter by default, [see here](https://developer.mozilla.org/zh-CN/docs/Web/CSS/backdrop-filter) for the opening method.

## Screenshots

### Internet Detector Status (Modified Feature)
The modified Argon theme now displays full internet status (Connected/Disconnected, VPN Status, Public IP) on the Overview page:

![Internet Detector Status](/Screenshots/internet_detector_status.png)

### Original Theme Styles
![desktop](/Screenshots/screenshot_pc.jpg)
![mobile](/Screenshots/screenshot_phone.jpg)

## Contributors

<a href="https://github.com/jerrykuku/luci-theme-argon/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=jerrykuku/luci-theme-argon&v=2" />
</a>

Made with [contrib.rocks](https://contrib.rocks).

## Related Projects

- [luci-app-argon-config](https://github.com/gonav8/luci-app-argon-config): Argon theme config plugin
- [openwrt-package](https://github.com/jerrykuku/openwrt-package): My OpenWrt package

## Credits

[luci-theme-material](https://github.com/LuttyYang/luci-theme-material/)
