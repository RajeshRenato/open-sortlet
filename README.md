# Sortlet

**Every inbox, sorted.** Sortlet is a desktop app that pulls mail from Gmail, Outlook, iCloud, Yahoo, Zoho or any IMAP
account, sorts it with Claude, and keeps it in a database on your own computer.

Website: https://RajeshRenato.github.io/open-sortlet/

## Download

Get the latest version from the [Releases](https://github.com/RajeshRenato/open-sortlet/releases/latest) page.

| Platform | File |
|----------|------|
| 🍎 macOS (Apple Silicon) | [`Sortlet-0.2.0-arm64.dmg`](https://github.com/RajeshRenato/open-sortlet/releases/latest/download/Sortlet-0.2.0-arm64.dmg) |
| 🍎 macOS (Intel) | [`Sortlet-0.2.0-x64.dmg`](https://github.com/RajeshRenato/open-sortlet/releases/latest/download/Sortlet-0.2.0-x64.dmg) |
| 🪟 Windows (Installer) | [`Sortlet-Setup-0.2.0.exe`](https://github.com/RajeshRenato/open-sortlet/releases/latest/download/Sortlet-Setup-0.2.0.exe) |
| 🪟 Windows (Portable) | [`Sortlet-0.2.0-portable.exe`](https://github.com/RajeshRenato/open-sortlet/releases/latest/download/Sortlet-0.2.0-portable.exe) |
| 🐧 Linux (AppImage x64) | [`Sortlet-0.2.0-x86_64.AppImage`](https://github.com/RajeshRenato/open-sortlet/releases/latest/download/Sortlet-0.2.0-x86_64.AppImage) |
| 🐧 Linux (AppImage arm64) | [`Sortlet-0.2.0-arm64.AppImage`](https://github.com/RajeshRenato/open-sortlet/releases/latest/download/Sortlet-0.2.0-arm64.AppImage) |
| 🐧 Linux (Debian x64) | [`Sortlet-0.2.0-amd64.deb`](https://github.com/RajeshRenato/open-sortlet/releases/latest/download/Sortlet-0.2.0-amd64.deb) |
| 🐧 Linux (Debian arm64) | [`Sortlet-0.2.0-arm64.deb`](https://github.com/RajeshRenato/open-sortlet/releases/latest/download/Sortlet-0.2.0-arm64.deb) |

## Install

### macOS

1. Download the `.dmg` for your Mac (Apple Silicon or Intel) and drag **Sortlet** to Applications.
2. The first time you open it, macOS blocks it because the app isn't notarized. Go to
   **System Settings → Privacy & Security** and click **Open Anyway**.
3. Click **Open** in the confirmation dialog. You only need to do this once.

### Windows

1. Download `Sortlet-Setup-0.2.0.exe` (or the portable `.exe` if you don't want to install).
2. If SmartScreen warns you, click **More info**, then **Run anyway**.
3. Follow the installer.

### Linux

```bash
# AppImage
chmod +x Sortlet-0.2.0-x86_64.AppImage
./Sortlet-0.2.0-x86_64.AppImage

# Debian / Ubuntu
sudo dpkg -i Sortlet-0.2.0-amd64.deb
```

## What it does

- **Connect any number of inboxes.** Gmail signs in with Google; everything else uses IMAP with an app password.
- **Sorts mail into your categories.** Uses Claude Code (your own login), the Claude API, or offline rules. Edit the
  categories in Settings; anything you sort by hand stays put.
- **Flags what needs you.** *Needs reply* when a person is waiting on your answer. *Needs attention* when something
  needs action, with the reason: a failed payment, an expiring card, a new sign-in, a changed flight.
- **Ask your mail.** "What needs my reply?", "Any invoices this week?", "Draft a reply to Daniel saying Thursday
  works." Answers link straight to the emails.
- **Works with Claude and Copilot.** While Sortlet is open, Claude Code, Claude Desktop and VS Code Copilot can search,
  sort and draft replies through MCP. Settings → Connect Claude / Copilot has the configs to copy.
- **Never sends mail.** Replies are saved to your Drafts folder for you to review and send.
- **Your data stays local.** Mail is stored on your computer, passwords and tokens are encrypted with your system
  keychain, and you can set emails to delete themselves after 7 to 365 days.

## Updates

Sortlet checks this repo for new versions at startup and every 6 hours. On Windows and Linux (AppImage) it updates
itself; on macOS it shows a Download button for the new version.

## License

MIT
