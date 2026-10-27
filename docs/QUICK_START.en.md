# Getting started with Nahang Crawl

[فارسی](QUICK_START.fa.md) · [Privacy](PRIVACY.en.md) · [Known limitations](KNOWN_LIMITATIONS.md) · [Report a problem](SUPPORT.md)

## Install and open

1. Download the Windows x64 package from the [official releases page](https://github.com/seotaheri-beep/nahang-crawl-releases/releases). No system-wide Node.js, Java or developer tools are required to run it.
2. If a release provides a Setup installer, run it. For a ZIP release, extract **all** files into a new folder and run `NahangCrawl.exe` there. Keep the executable together with its accompanying files.
3. Current packages are beta builds without a digital signature. Verify the source and SHA-256 against that release. This guide does not require disabling Windows security protections.
4. A downloadable release may differ from an internal test candidate. Check the version shown at the bottom of the window against the release notes.

There is one edition and no licence activation or free/paid split in this version. A first crawl needs no Google account or API key. Press **F1** for the offline user guide.

## Your first crawl

1. Enter a full address such as `https://example.com/` in the toolbar. Choose a site you are authorised to inspect.
2. Keep **Spider** mode and **Subdomain** scope. Domain and Subfolder change the scope. Start with the **500 URL limit**, two concurrent requests and the default delay.
3. Choose **Start Crawl**. Use F7 to pause, F9 to resume and F8 to stop. Results appear as pages arrive.
4. Select a row in Internal. The lower panel shows URL details, links and captured evidence. Tab can enter the result rows; Enter selects a row, and Up/Down move between rows.
5. Reaching the limit means some URLs were not crawled. Change limits for a fresh run. Resuming uses that crawl’s saved configuration.

For a JavaScript-dependent site, enable rendering under **Configuration → Crawl Config → Spider → Rendering** before a fresh run. The Embedded Browser must be enabled. Rendering uses more resources and does not guarantee complete lazy loading or website interactions.

## Reports and exports

- The tab, filter, search and Segment narrow the current view. An empty table does not always mean no data exists.
- **Export CSV** produces a spreadsheet file. **Bulk Export → Multi-Export** saves several selected reports and files together.
- **Reports** contains overview and specialist reports. Pause or complete a crawl before running post-crawl checks with **Crawl Analysis → Start**.
- Reports use saved evidence. Missing PageSpeed, rendering, headers or accessibility evidence does not imply a clean result.
- noindex, canonical declarations and empty alt text may be intentional. Interpret each finding in the context of the page.

## Save, reopen and back up

| Need | Command |
|---|---|
| Reopen an existing run | File → Crawls, or Ctrl+O |
| Save a reopenable file | File → Export → Crawl File, or Ctrl+Shift+S; `.nahang-crawl` extension |
| Import a crawl file | File → Import, or Ctrl+Shift+O |
| Create a backup | File → Backup and Transfer |
| Start a fresh view | File → New, or Ctrl+N; existing runs stay in history |

**Database** saves changes as you work. In **RAM** mode, press **Ctrl+S** before quitting. CSV is not a saved RAM session or a backup. App data normally lives under `%APPDATA%\NahangCrawl`; inspect the active database path in Application Settings → Storage Mode. Changing the directory does not automatically move or merge previous files. Automatic Crawl Retention defaults to Never; changing it may delete old runs covered by that policy.

Before upgrading, make a backup and finish active operations. Extract a newer ZIP into a separate folder and preserve the user data directory. **Help → Check for Updates** checks published versions. Auto Check is optional and off by default. Downloading and running an installer remain user actions.

## Settings and troubleshooting

Find Persian/English, theme, accent colour and Focus Mode in **File → Settings**. Application preferences are separate from a crawl’s configuration. Storage, Memory and some network/browser changes require a later app start; follow the message in that section.

If only one URL appears, inspect its status and redirect destination. Proxy, robots.txt, scope, Include/Exclude and limits may explain it. A login page or security challenge may be returned instead of the site. Review network settings before changing them.

For empty API reports, check the date range, Property and available source data. A successful GA4 connection does not guarantee traffic data. A quota error is a provider restriction. Ollama needs a running local server and an appropriate installed local model; the app does not automatically download models.

For a problem report, record the version and reproduction steps, then use **Help → Debug → Save Logs**. See [Support](SUPPORT.md) before sharing diagnostics publicly.
