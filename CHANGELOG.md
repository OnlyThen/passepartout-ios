# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 1.8.0 (2019-08-01)

### Added

- "Custom DNS" preset for Mullvad. [api-source-mullvad#1](https://github.com/passepartoutvpn/api-source-mullvad/issues/1)
- Change app language from Settings in iOS 13. [#90](https://github.com/passepartoutvpn/passepartout-ios/issues/90)

### Changed

- Disconnect on "No buffer space available" rather than leaving a stale connection (improve later). [tunnelkit#104](https://github.com/passepartoutvpn/tunnelkit/issues/104)

### Fixed

- VPN staying active while it's not. [tunnelkit#106](https://github.com/passepartoutvpn/tunnelkit/issues/106)
- Disconnection on renegotiation. [tunnelkit#105](https://github.com/passepartoutvpn/tunnelkit/issues/105)
- Support third party apps when sending e-mails.
- Refreshed infrastructures are not retained. [passepartout-core-apple#1](https://github.com/passepartoutvpn/passepartout-core-apple/issues/1)
- Portuguese bound to Brazil region.
- German spelling of "Default gateway".
- Some French wording (Joel Gallant).
- Erroneous placeholders in Network Settings (Joel Gallant).

## 1.7.0 (2019-06-02)

### Added

- Dutch translations (Norbert de Vreede). [#81](https://github.com/passepartoutvpn/passepartout-ios/pull/81)
- Greek translations (Konstantinos Koukoulakis).
- French translations (Julien Laniel).
- Spanish translations (Davide De Rosa, Elena Vivó).
- Swedish translations (Henry Gross-Hellsen). [#82](https://github.com/passepartoutvpn/passepartout-ios/pull/82)

## 1.6.1 (2019-05-20)

### Added

- Override network settings. [#77](https://github.com/passepartoutvpn/passepartout-ios/pull/77)
- Support for `--redirect-gateway block-local` (partial). [tunnelkit#81](https://github.com/passepartoutvpn/tunnelkit/issues/81)
- Russian translations (Alexander Korobynikov).

### Changed

- Host compression framing and algorithm are now editable.

### Fixed

- NordVPN double servers not connecting out of the box. [#78](https://github.com/passepartoutvpn/passepartout-ios/issues/78)
- Authentication with OpenVPN AS. [tunnelkit#95](https://github.com/passepartoutvpn/tunnelkit/issues/95)
- TLS failed with some servers. [tunnelkit#97](https://github.com/passepartoutvpn/tunnelkit/issues/97)

## 1.6.0 (2019-05-01)

### Added

- VyprVPN provider. [#72](https://github.com/passepartoutvpn/passepartout-ios/pull/72)
- More infrastructure metadata.
- Portuguese translations (Helder Santana). [#70](https://github.com/passepartoutvpn/passepartout-ios/pull/70)
- German translations (Christian Lederer).
- Russian translations (Alexander Korobynikov).

### Changed

- Do not redirect all traffic to VPN unless `--redirect-gateway` specified. [#71](https://github.com/passepartoutvpn/passepartout-ios/pull/71)

### Fixed

- Fall back to CloudFlare DNS when no servers provided. [tunnelkit#84](https://github.com/passepartoutvpn/tunnelkit/issues/84)
- UDP may disconnect on high speeds. [tunnelkit#87](https://github.com/passepartoutvpn/tunnelkit/issues/87)
- SoftEther connects without VPN icon. [#69](https://github.com/passepartoutvpn/passepartout-ios/issues/69)
- Misleading Mullvad password suggestion. [#75](https://github.com/passepartoutvpn/passepartout-ios/issues/75)
- Leave digest editable despite cipher. [#74](https://github.com/passepartoutvpn/passepartout-ios/issues/74)
- TLS errors with passphrase-protected .ovpn profiles. [tunnelkit#91](https://github.com/passepartoutvpn/tunnelkit/issues/91)
- Issue with DNS-only VPN profiles. [#73](https://github.com/passepartoutvpn/passepartout-ios/issues/73)

## 1.5.0 (2019-04-17)

### Added

- NordVPN provider. [#65](https://github.com/passepartoutvpn/passepartout-ios/pull/65)
- Support for `dhcp-option PROXY_HTTP[S]`. [tunnelkit#74](https://github.com/passepartoutvpn/tunnelkit/issues/74)

### Fixed

- Regression in DNS configuration. [#68](https://github.com/passepartoutvpn/passepartout-ios/issues/68)
- SoftEther timing out. [tunnelkit#67](https://github.com/passepartoutvpn/tunnelkit/issues/67)
- VPN status cell doesn't always enter active profile. [#63](https://github.com/passepartoutvpn/passepartout-ios/issues/63)
- Masking preference not retained. [#64](https://github.com/passepartoutvpn/passepartout-ios/issues/64)
- Issues with very long PUSH_REPLY. [tunnelkit#71](https://github.com/passepartoutvpn/tunnelkit/issues/71)
- Missing app icon in Credits.

## 1.4.0 (2019-04-11)

### Added

- ProtonVPN provider. [#7](https://github.com/passepartoutvpn/passepartout-ios/issues/7)
- Italian translations. [#58](https://github.com/passepartoutvpn/passepartout-ios/pull/58)
- In-app donations.
- Provider logos. [#55](https://github.com/passepartoutvpn/passepartout-ios/pull/55)
- Country flags. [#56](https://github.com/passepartoutvpn/passepartout-ios/pull/56)
- VPN status shortcut, enters active profile on selection.

### Changed

- Automatic protocol defaults to UDP endpoints. [#61](https://github.com/passepartoutvpn/passepartout-ios/pull/61)
- Improved Account screen, footers were hardly tappable.

### Fixed

- Some providers may crash on VPN activation. [#57](https://github.com/passepartoutvpn/passepartout-ios/issues/57)
- Mullvad dying due to ping timeout. [#62](https://github.com/passepartoutvpn/passepartout-ios/issues/62)
- Pushing DOMAIN has no effect. [#48](https://github.com/passepartoutvpn/passepartout-ios/issues/48)

## 1.3.0 (2019-04-03)

### Added

- Windscribe provider. [#39](https://github.com/passepartoutvpn/passepartout-ios/issues/39)

### Fixed

- Support PKCS#8 encrypted cert keys. [#43](https://github.com/passepartoutvpn/passepartout-ios/issues/43)
- Handle PEM with preamble. [tunnelkit#78](https://github.com/passepartoutvpn/tunnelkit/issues/78)
- Infrastructures not retained after refresh. [#54](https://github.com/passepartoutvpn/passepartout-ios/issues/54)

## 1.2.0 (2019-04-01)

### Added

- Siri Shortcuts in-app manager. [#46](https://github.com/passepartoutvpn/passepartout-ios/pull/46)
- Background data count updates in diagnostics. [#51](https://github.com/passepartoutvpn/passepartout-ios/pull/51)
- Configure masking in debug log for improved diagnostics.
- Mullvad provider. [#45](https://github.com/passepartoutvpn/passepartout-ios/pull/45)
- Support for encrypted certificate private keys. [#43](https://github.com/passepartoutvpn/passepartout-ios/pull/43)

### Changed

- Upgraded to Swift 5.

### Fixed

- EKU not verified with providers (regression).
- Occasionally overlapping footers in organizer.

## 1.1.0 (2019-03-22)

### Added

- Support for LZO compression. [#32](https://github.com/passepartoutvpn/passepartout-ios/issues/32)
- Siri shortcuts. [#41](https://github.com/passepartoutvpn/passepartout-ios/pull/41)
- Custom intents, have a look at Spotlight suggestions for Passepartout. [#40](https://github.com/passepartoutvpn/passepartout-ios/pull/40)
- TunnelBear provider. [#35](https://github.com/passepartoutvpn/passepartout-ios/pull/35)

### Changed

- Normalize localization of provider locations.

### Fixed

- Profile not activating if none is active. [#42](https://github.com/passepartoutvpn/passepartout-ios/issues/42)
- EKU verification enabled when it shouldn't be.
- Incorrect VPN status after renaming. [#37](https://github.com/passepartoutvpn/passepartout-ios/issues/37)
- Profile change doesn't disconnect active VPN. [#38](https://github.com/passepartoutvpn/passepartout-ios/issues/38)
- Some reconnection issues encountered with TunnelBear and NordVPN.
- Hosts gone while connected (credit to Aston Martin). [#19](https://github.com/passepartoutvpn/passepartout-ios/issues/19)

## 1.0.3 (2019-03-06)

### Fixed

- Regression in profile activation. [#36](https://github.com/passepartoutvpn/passepartout-ios/issues/36)

## 1.0.2 (2019-03-04)

### Fixed

- Profile sometimes not connecting right after add.
- Custom DNS servers were not applied.
- Shut down if server uses compression at all.
- Broken link to SwiftGen license.

## 1.0.1 (2019-02-27)

### Added

- Override DNS servers via `dhcp-option DNS`. [tunnelkit#56](https://github.com/passepartoutvpn/tunnelkit/pull/56)
- About link to FAQ.

### Changed

- Only enable EKU verification if `remote-cert-tls server`. [tunnelkit#64](https://github.com/passepartoutvpn/tunnelkit/pull/64)

### Fixed

- Shut down if server pushes a compression directive. [tunnelkit#65](https://github.com/passepartoutvpn/tunnelkit/pull/65)
- Retain DNS reply order in resolved endpoint addresses. [#31](https://github.com/passepartoutvpn/passepartout-ios/pull/31)

## 1.0 (2019-01-16)

### Added

- Automated app rating mechanism.
- Dot as a legal character in host profile title. [#22](https://github.com/passepartoutvpn/passepartout-ios/issues/22)
- Host profiles can now be renamed. [#24](https://github.com/passepartoutvpn/passepartout-ios/issues/24)
- Explicit rejection of encrypted client certificate keys. [#15](https://github.com/passepartoutvpn/passepartout-ios/issues/15)
- Attach .ovpn when reporting a connectivity issue, stripped of sensitive data. [#13](https://github.com/passepartoutvpn/passepartout-ios/pull/13)
- iTunes File Sharing (skythedesu). [#14](https://github.com/passepartoutvpn/passepartout-ios/pull/14)
- Tunnel failure reporting in UI. [#8](https://github.com/passepartoutvpn/passepartout-ios/pull/8)
- Explicit "Reconnect" button. [#9](https://github.com/passepartoutvpn/passepartout-ios/pull/9)
- Option to revert host parameters to original configuration (Nicholas Caito). [#10](https://github.com/passepartoutvpn/passepartout-ios/pull/10)
- Support for TLS wrapping (tls-auth and tls-crypt). [#5](https://github.com/passepartoutvpn/passepartout-ios/pull/5)
- AES-GCM and new endpoints to PIA network preset. [tunnelkit#32](https://github.com/passepartoutvpn/tunnelkit/pull/32)
- Disclosure indicators in profile organizer (Samuel Michaels).
- Disclaimer for app usage.

### Removed

- "Test connectivity" until it's more transparent.
- Password confirmation field, redundant with authentication failure message.

### Changed

- Relocated API endpoints, better before first release.
- Reorganized credits page.
- Internal refactoring (nothing visible).
- Disconnect VPN by default when entering a trusted network. [#25](https://github.com/passepartoutvpn/passepartout-ios/pull/25)
- Host parameters are read-only if there isn't an original configuration to revert to.
- Overall serialization performance.
- Drive generic support requests on Reddit.
- Add current Wi-Fi to trusted networks list but don't trust it by default.

### Fixed

- Infrastructures not refreshed. [#29](https://github.com/passepartoutvpn/passepartout-ios/issues/29)
- Incorrect compression warnings when importing host configurations. [#20](https://github.com/passepartoutvpn/passepartout-ios/pull/20)
- Regression in provider endpoints, IPv4 appearing reversed. [#23](https://github.com/passepartoutvpn/passepartout-ios/pull/23)
- Handling of extra whitespaces in .ovpn (Mike Mayer). [#17](https://github.com/passepartoutvpn/passepartout-ios/issues/17)
- Glitches in import wizard flow, sometimes not even appearing.
- Warn about .ovpn containing potentially unsupported compression. [#16](https://github.com/passepartoutvpn/passepartout-ios/issues/16)
- Retain credentials of replaced host profile.
- Original configuration not saved after reset.
- Connection occasionally turning inactive after a while.
- Improved performance and privacy of debug log.
- .ovpn files could not be imported without OpenVPN Connect installed. [#6](https://github.com/passepartoutvpn/passepartout-ios/issues/6)
- Fixed Mullvad abrupt disconnection. [tunnelkit#30](https://github.com/passepartoutvpn/tunnelkit/issues/30)
- Credentials are now optional for host profiles. [#4](https://github.com/passepartoutvpn/passepartout-ios/pull/4)
- Can now import .ovpn files from Apple Files app. [#1](https://github.com/passepartoutvpn/passepartout-ios/pull/1)
- Reject unrecognized values for `cipher`, `auth` and `proto`. [#1](https://github.com/passepartoutvpn/passepartout-ios/pull/1)
- Alert unsupported configuration options.
- Use accent color for checkmarks in table cells.

## 1.0 beta 975 (2018-10-11)

First public beta release.
