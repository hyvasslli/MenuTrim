# Release Process / 发布流程

This document contains only the public release checklist. Credentials, signing identities, account details, and local key paths must remain outside this repository.

本文仅记录可公开的发布检查表。凭据、签名身份、账户资料和本机密钥路径不得写入本仓库。

1. Complete and verify development in the private source repository.
2. Produce a Release build.
3. Sign the app and DMG with the appropriate Developer ID identities.
4. Submit the package for Apple notarization.
5. Staple the notarization ticket to the distributed package.
6. Verify the app and DMG with codesign, spctl, and stapler.
7. Calculate the DMG SHA-256 checksum.
8. Create a release in this public product repository.
9. Upload MenuTrim-x.y.z.dmg and its checksum.
10. Write release notes and update CHANGELOG.md.
11. Download the uploaded asset once and repeat the signature, notarization, stapling, and checksum checks.

Never commit certificates, private keys, notarization credentials, App Store Connect API keys, provisioning profiles, or signing passwords.
