# Beta acceptance — 1.0.0-beta.1

Windows x64 prerelease, unsigned. Reviewed 2026-10-28.

- Source revision: `5b4f89d981f34283b5d35a11884614bf45e1b67d` (maintained in the private source repository).
- Compiled entrypoint/UI fingerprint: `7041688150c80baad937edbeb9db663327df320bc65f92f2c4a05ed2ae0b6e5f`.
- Fresh Windows GitHub CI: 143 files, **1432 passing tests**, zero failures/skips/deferred tests.
- Native desktop, security boundaries/encrypted storage and Chromium rendering regressions: passed.
- ZIP, Setup, Squirrel package/feed: all four hashes match the build manifest.
- Portable contents: all **2271 files** match the accepted manifest; 10 public documents included.
- Developer OAuth client: absent from this public beta.
- Upgrade from the published alpha.136 portable: saved pages and synthetic encrypted credentials preserved.
- Setup install, upgrade, uninstall preserving user data, and reinstall/reopen: passed. The earlier installer used for the installer upgrade check is a metadata-only fixture, not a historical public Setup.
- Unicode/space paths, Start Menu/Desktop shortcuts and bundled Java/LanguageTool: passed.

The app's PATH excluded node, pnpm, java and javac. The fresh GitHub-hosted Windows machine itself contains development tools; this is not a claim that every consumer Windows version or policy was tested. Packages are unsigned and bundle Electron 46.0.0-alpha.1.

The release downloads are the same accepted artifact bytes, not a rebuild after acceptance. Use SHA256SUMS.txt and release-manifest.json on the release page to verify files.

Independent beta user feedback is pending. See [the test checklist](docs/BETA_TESTING.md), [known limitations](docs/KNOWN_LIMITATIONS.md) and [support](docs/SUPPORT.md). No private profiles, tokens or raw user crawls are included in this report.

گزارش پذیرش: آزمون‌های خودکار و نصب/ارتقای Windows موفق‌اند؛ بازخورد کاربران بیرونی هنوز دریافت نشده است. بسته بدون امضا و runtime آلفاست؛ حدود محیط آزمایش و مراحل بازتولید در راهنما آمده‌اند.
