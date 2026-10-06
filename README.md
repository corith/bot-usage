<p align="center">
  <img src="Artwork/READMEHero.png" alt="A friendly menu-bar robot presenting Codex usage charts" width="760">
</p>

# BotUsage

Codex usage, one click from your Mac's menu bar.

BotUsage shows your quota windows, official daily token totals, and local token activity by model. It stays out of the Dock, refreshes while it runs, and offers four themes: macOS, Omarchy, Codex, and Demon.

**[Download the latest release](https://github.com/corith/bot-usage/releases/latest)** · **[Release notes](https://github.com/corith/bot-usage/releases)** · **[Report an issue](https://github.com/corith/bot-usage/issues)**

## Requirements

- **macOS 14 Sonoma or later**, on Apple silicon or Intel. One universal download supports both.
- **Codex Desktop or the Codex CLI**, installed and signed in to ChatGPT.

## Install

1. Download **[BotUsage 0.2.6](https://github.com/corith/bot-usage/releases/download/v0.2.6/BotUsage-v0.2.6-macos-universal.zip)**, or choose a newer version from [Releases](https://github.com/corith/bot-usage/releases/latest).
2. Unzip the download and move **BotUsage.app** to **Applications**.
3. Open the app. Use the bot icon in the menu bar to view your usage.

### First launch

Version 0.2.6 is **Developer ID signed and notarized by Apple**, with the notarization ticket attached to the app.

macOS may ask you to confirm that you want to open an app downloaded from the internet. Choose **Open** to continue. See [Apple's guidance on opening downloaded apps](https://support.apple.com/102445).

## Updates

Open the **Settings** gear in the panel footer and choose **Check for Updates…**. You can also opt in to automatic update checks in Settings.

Updates use Sparkle and this public repository. **No GitHub account or access token is required.** Sparkle checks the signed update feed and verifies the downloaded update before installing and relaunching BotUsage. If you already use 0.2.5, you can update to 0.2.6 from Settings.

**Upgrading from 0.2.4 or earlier?** Download and install the latest version manually once. Earlier builds check the previous private repository; 0.2.5 and later use this public update channel.

## Reading your usage

- **Quota windows** show Codex's reported allowance and reset times. Hover for details.
- **Official daily totals** come from your signed-in Codex account, when available.
- **Local raw activity** comes from Codex session history on this Mac, including archived sessions. It shows recent activity and model breakdowns, so it can differ from account-wide official totals.

Raw tokens are input plus output, including cached input. Repeated use of conversation context counts again. **Fresh** tokens exclude cached input. Local token counts are diagnostic activity totals, not a bill or a measure of remaining subscription allowance. Missing or unreadable history can produce incomplete totals; BotUsage displays a warning when it detects this.

BotUsage uses your installed Codex and its existing sign-in to request account data. It also reads local session history. It contacts GitHub for update checks and downloads.

## Make it yours

Choose a theme from the panel's dropdown or **Settings → Theme**. Enable **Open at Login** in Settings to start BotUsage when you sign in to your Mac; keep the app in Applications first.

Data normally refreshes every five minutes. Opening the panel or waking your Mac refreshes data that is more than a minute old. Use the refresh button to retry sooner. If official usage is unavailable, confirm that Codex is installed and signed in, then refresh again.

## Support

[Open an issue](https://github.com/corith/bot-usage/issues) with your BotUsage version, macOS version, and a description of what happened. Please remove account details and other personal information from screenshots or logs.

This repository hosts public downloads, release notes, and support. BotUsage's application source remains private. See [third-party notices](THIRD-PARTY-NOTICES.md) for the components included in the app.
