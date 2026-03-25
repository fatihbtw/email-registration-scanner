# 📋 Email Registration Scanner

An [OpenClaw](https://openclaw.ai) skill that scans your email accounts for registration, welcome, and confirmation emails — and builds a deduplicated, chronological list of every service you've ever signed up for.

## Supported Providers

| Provider | Access |
|---|---|
| Gmail | Gmail MCP connector |
| iCloud Mail | IMAP |
| Outlook / Hotmail / Live | IMAP |
| Yahoo Mail | IMAP |
| AOL Mail | IMAP |
| GMX | IMAP |
| Web.de | IMAP |
| T-Online | IMAP |
| Fastmail | IMAP |
| Proton Mail | IMAP via Bridge |

## Supported Languages

English · Deutsch · Français · Español · Italiano · Português · Nederlands · Polski · Türkçe

## Installation

```bash
# Option 1 – via OpenClaw directly (paste this URL into your agent chat)
https://github.com/fatihbtw/email-registration-scanner

# Option 2 – manual
mkdir -p ~/.openclaw/skills/email-registration-scanner
cp -r . ~/.openclaw/skills/email-registration-scanner
```

## Usage

Just tell your OpenClaw agent:
- *"Scan my emails for registrations"*
- *"Where am I registered?"*
- *"Wo bin ich überall registriert?"*
- *"/registration-scanner"*

## File Structure

```
email-registration-scanner/
├── SKILL.md                        # Core workflow
├── references/
│   ├── providers.md                # IMAP settings + app password guides
│   └── search-queries.md          # Search terms in 9 languages
└── scripts/
    └── imap_scan.py               # Python IMAP scanner (stdlib only)
```

## Privacy & Security

- Credentials are never stored or logged
- All processing happens locally on your machine
- Temp files are deleted after each session
- Uses app-specific passwords (not your main account password)

## License

MIT
