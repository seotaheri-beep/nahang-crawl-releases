# Privacy and data flow

This document describes the current technical behaviour of Nahang Crawl. [فارسی](PRIVACY.fa.md). Reviewed: 2026-10-27. This local document is not yet a published, approved Google OAuth privacy-policy URL.

## Data on your device

Crawl databases, queues, URLs, findings, extracted content, enabled HTML/DOM/PDF and screenshot captures, settings, history and usage statistics live in local app storage or your chosen storage directory. Exports and backups are saved to locations you select. Summary/Usage statistics are recorded locally and are not automatically uploaded.

Database mode saves as you work; RAM sessions require saving. Reports may create temporary disk snapshots. Deleting a crawl does not necessarily delete independently saved exports, backups, temporary files or previous aggregate usage statistics. See the [guide](QUICK_START.en.md) for storage and recovery. Retention defaults to Never and does not cover exports you saved separately.

Passwords, keys, Google tokens and authentication data use the operating system’s secure storage. Availability depends on the system and associated profile. Treat profiles and backups as private data. Captured pages and exports may contain private site content. Credential-vault encryption does not mean the entire crawl file is encrypted.

## Data sent outside the device

| Action | Destination and data |
|---|---|
| HTML/JavaScript crawl and resources | Sites allowed by the configuration; URL, User-Agent, connection IP and any configured request headers/cookies or required login data |
| Search Console / GA4 | Google with the user’s read-only permission; Property, dates, required dimensions/filters and connection credentials. Responses are stored locally |
| PageSpeed | Google PageSpeed; public URL and strategy, plus a key only if configured |
| Gemini | Google; the analysis instruction, bounded page text, title and URL with the user’s key, when analysis is run |
| Moz | Moz; selected URLs and the user’s key for metrics |
| Ollama / Embeddings | Local loopback models; selected text for inference or embeddings. Cloud models are not accepted by this integration |
| Check for Updates | GitHub and official asset download hosts; release/asset requests and ordinary network connection metadata. Automatic checks are optional and off by default |
| Optional email notifications | The selected account/SMTP provider and configured recipients; completion messages and selected attachments |
| MCP | An authorised client after the server is started; data and results exposed by permitted tools |

External providers’ policies apply to data you send them. Your Proxy and trusted-certificate choices also affect connection routing and validation. Optional service accounts are not required for an ordinary crawl.

## Diagnostics and sharing

Technical logs use permitted events and fields, with rotation and size limits. Normal events deliberately omit page bodies, passwords, keys, cookies and authentication headers. Debug Options controls logging levels. Save Logs creates a local file; it does not automatically send it to support. Usage Stats → Share also creates local CSV/JSON files. Review files before sharing them.

CSV, crawl files, captured HTML, screenshots and backups can contain URLs, page contents or private project data. Do not post these publicly without permission. See [Support](SUPPORT.md) for a report template that avoids credentials.

Disconnecting Google in the app removes the local connection credentials. Revoking access in Google account settings is a separate action. Manage independently saved copies yourself after changing the storage location or deleting a crawl.
