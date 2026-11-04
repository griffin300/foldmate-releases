# Foldmate (Windows, with a Mac preview)

Foldmate runs AI models on your own PC. You don't need an account, and your chats stay on your computer
unless you choose a cloud model.

- **Your chats are encrypted on your disk**, with a key protected by your Windows account.
- **No telemetry or analytics.** Foldmate doesn't report what you do, and it never sends a support report for you.
- **Models run on this PC.** A cloud model is only used when you pick one, and Foldmate asks before it sends an existing chat.
- **Web research goes direct by default.** Turn on **Through Tor** for the private route. It never falls back to direct.
- **You decide what it may do.** Each chat has an approval mode: Ask every time, Approve for me, or Full access.

It can also research the web, use your desktop for you (computer use), run PC commands, code with OpenCode,
send email through connected services such as Gmail and Outlook, and let a paired iPhone use it through Tor or
over your own Wi-Fi. Press **Alt+\`** to open the chat bar.

The latest version is **1.1.17**.

**On this page:** [Install](#install) · [Mac (preview)](#mac-preview) · [What you need](#what-you-need) ·
[Privacy](#privacy-what-goes-online-and-when) · [Updates](#updates) · [Troubleshooting and FAQ](#troubleshooting-and-faq) ·
[Help and support](#help-and-support)

## New in 1.1.17

- **Smarter computer use:** the assistant now uses an exact calculator for totals with tax or delivery, price comparisons and free calendar times, and it touches nothing on screen, so it asks for no approval card. In our tests with the 27B model, pass rates were the same or better and tasks took about 11% less time on average.

Notes for earlier versions are in the [changelog](CHANGELOG.md). Older versions' notes are on the [Releases](https://github.com/griffin300/foldmate-releases/releases) page.

## Install

1. Open the **latest release** on this page and download `Foldmate-Setup-1.1.17.exe` under **Assets**.
2. Run it. Foldmate isn't code-signed yet, so Windows may stop it:
   - **"Windows protected your PC"** (SmartScreen): click **More info**, then **Run anyway**.
   - **Smart App Control** (on some new Windows 11 PCs): it blocks apps that aren't signed and doesn't offer
     Run anyway, so Foldmate can't run while it's on. Whether to turn it off is up to you. Read Microsoft's
     guidance first: on many PCs it can't be turned back on without resetting Windows.
3. The installer sets up what Foldmate needs:
   - Microsoft's Visual C++ runtime, if your PC doesn't have it;
   - Windows Subsystem for Linux (WSL), which Foldmate's web research engine runs in, if your PC doesn't have it.
     Windows downloads it from Microsoft.

   Windows may ask for permission (up to twice). A restart may be needed.
4. Foldmate opens. Its AI engine comes with it, and web research finishes setting up in the background
   during the first few minutes. Foldmate recommends a model that fits your PC and downloads it only when
   you choose **Download and load**. Models already in LM Studio's or Ollama's folders show up in
   **Models** where they are; nothing is copied.

## Mac (preview)

The Mac preview is version 1.1.15: download `Foldmate-1.1.15-mac.dmg` from the [1.1.15 release](https://github.com/griffin300/foldmate-releases/releases/tag/v1.1.15). It's built
and tested on Apple silicon (an M1). It isn't notarized by Apple yet, so macOS stops it the first time:
Control-click Foldmate in Applications and choose **Open**, or open **System Settings › Privacy & Security** and
choose **Open Anyway**. Some features are Windows-only for now, including PC commands and the phone's video and
computer sound.

## What you need

- **Windows 11, 64-bit.** Windows 11 is supported. Windows 10 may work, but it isn't supported. On a PC
  with an ARM processor, chat works but web research doesn't.
- **RAM:** 16 GB or more is recommended. 8 GB works with small models.
- **Virtualization turned on** in your PC's BIOS/UEFI, for web research. Without it chat still works, and
  Foldmate tells you which setting to turn on.
- **Disk:** about 15 GB free to install and set up, plus your models. A small model is about 1–2 GB.
- **A graphics card is optional.** Models run on the processor too, just more slowly.

## Privacy: what goes online, and when

Nothing you type leaves this PC unless you choose a cloud model or a connected service. These do go online:

| What | When | Route |
|---|---|---|
| Web research | A bot searches or reads a page | Direct by default (sites see your IP address and what you search), or Through Tor |
| Model search and downloads | You search in Models or click Download | Direct by default (Hugging Face sees your IP address), or Through Tor |
| Engines, add-ons and natural voices | You choose to install one | The same route as models |
| Cloud models and OpenCode Zen | Only when you pick one | Direct by default, or Through Tor, per provider |
| Connected services (Gmail, Outlook and Microsoft 365, MCP servers) | A bot uses one you added | Direct by default, or Through Tor |
| Your phone | While Remote is on | Tor (private link), your Wi-Fi (Same Wi-Fi connection), or your Tailscale network |
| Update checks | In the background | Directly to this page's releases (GitHub sees your IP address). Downloading and installing each need your click |

**Settings & tools › This computer › Local-only lockdown** stops all of it at once. Chat with your local
model keeps working. Foldmate's Help (**F1 › Privacy**) has the full list.

## Updates

Foldmate checks this page for new versions directly, not through Tor. Only releases signed with Foldmate's key
install, and each file is checked before it's used. When an update is available, a small arrow appears next to
Foldmate's name in the sidebar. Choose it to download the update, then choose **Restart to update**.

From 0.4.0 on, most updates download only the files that changed. 1.1.17 is one of those: from 1.1.16, 1.1.15 or 1.1.14 it's a
small download (about 19 MB). From an older version, the update downloads the full installer (about 0.88 GB).

## Troubleshooting and FAQ

### Windows says "Windows protected your PC". What do I do?

Foldmate isn't code-signed yet, so Windows SmartScreen may stop the installer with this message.
Click **More info**, then **Run anyway**.

### Windows blocks the installer and there's no Run anyway button.

That's **Smart App Control**, which is on for some new Windows 11 PCs. It blocks apps that aren't signed, so
Foldmate can't run while it's on. Whether to turn it off is up to you. Read Microsoft's guidance first: on many
PCs it can't be turned back on without resetting Windows.

### Chat works, but web research doesn't.

Web research runs in Windows Subsystem for Linux (WSL), and it needs virtualization turned on in your PC's
BIOS/UEFI. Without it, chat still works, and Foldmate tells you which setting to turn on. On a PC with an ARM
processor, chat works but web research doesn't. Right after you install, web research may still be setting up:
it finishes in the background during the first few minutes. OpenCode needs WSL and virtualization too.

### How do updates work?

Foldmate checks this page for new versions in the background. When one is ready, a small arrow appears next to
Foldmate's name in the sidebar. Choose it to download the update, then choose **Restart to update**. Downloading
and installing each need your click. Most updates download only the files that changed: 1.1.17 is about 19 MB
from 1.1.16, 1.1.15 or 1.1.14.
From an older version, the update downloads the full installer (about 0.88 GB). Only releases signed with
Foldmate's key install, and each file is checked before it's used. See [Updates](#updates).

### Is there a Mac version?

Yes, as a preview. It's version 1.1.15, built and tested on Apple silicon (an M1). Download
`Foldmate-1.1.15-mac.dmg` from the [1.1.15 release](https://github.com/griffin300/foldmate-releases/releases/tag/v1.1.15).
It isn't notarized by Apple yet, so macOS stops it the first time: Control-click Foldmate in Applications and
choose **Open**, or open **System Settings › Privacy & Security** and choose **Open Anyway**. Some features are
Windows-only for now, including computer use, Share control, the screen-saver handling for your phone, PC
commands, and the phone's video and computer sound.

### What changes when I turn on Through Tor?

- **Web research:** by default it goes direct, and sites see your IP address and what you search. Through Tor
  is the private route. It never falls back to direct.
- **Model downloads, cloud models and connected services:** each can go direct (the default) or Through Tor.
  For cloud models, you choose per provider.
- **Update checks** go directly to this page's releases, not through Tor. GitHub sees your IP address.
- **Your phone:** Remote works through Tor with no account, or straight over your own Wi-Fi. On the same Wi-Fi,
  you hear this computer at full quality (48 kHz stereo). Over Tor, sound goes up to 9.6 kHz.

### How do I stop everything from going online?

Turn on **Settings & tools › This computer › Local-only lockdown**. It stops everything in the
[privacy table](#privacy-what-goes-online-and-when) at once. Chat with your local model keeps working.

### Do I need a graphics card?

No. Models run on the processor too, just more slowly. 16 GB of RAM or more is recommended, and 8 GB works
with small models.

### Can I use models I already downloaded for LM Studio or Ollama?

Yes. Models already in LM Studio's or Ollama's folders show up in **Models** where they are. Nothing is copied.

## Asking before it acts

Each chat has an approval mode:

- **Ask every time:** every action on your PC shows a card first.
- **Approve for me:** reading your screen, and OpenCode's work inside its project's sealed box, run without
  asking. Clicks, typing, deleting and browser steps still ask. An optional switch (off by default) lets this
  PC's model approve routine steps that are clearly what you asked for.
- **Full access:** Foldmate uses your PC without asking first. Steps in protected windows still ask: password
  managers, Windows Security and Settings, sign-in and User Account Control prompts, Task Manager and the
  Registry Editor. PC commands that download or install software still show a card, and every action is
  recorded in the chat. Use it only in chats where you trust what the model is doing.
- **Purchases with the Wallet** ask you first in every mode, unless you allow purchases within your limits in
  Full access (off by default).

## The tray, the chat bar and Assist

- **The tray:** right-click Foldmate's icon by the clock for **Open Foldmate**, **Load model**, **Lens**,
  **Eject model**, **App settings** and **Quit Foldmate**. Quit unloads the model and stops web research, so
  their memory is free again.
- **The chat bar:** press **Alt+\`** (the key under Esc). Alt+Space, Ctrl+Alt+F and Ctrl+Alt+B are choices in
  **App settings › This computer**. Text you highlight while it's open joins your question.
- **Assist:** select text in any app and press **Ctrl+Alt+Space** to proofread, rewrite, summarize, explain or
  translate it with your own model, or search the web about it.

## Your phone (beta)

**Settings & tools › Remote** lets a paired phone use Foldmate on this PC: through Tor with no account, or
straight over your own Wi-Fi. It's off until you turn it on. To pair, install Foldmate on your iPhone from the
App Store, open Remote there and scan the code Foldmate shows. A phone browser over Tailscale works too:
**Remote › Advanced**.

## Uninstall

Use **Settings › Apps › Installed apps › Foldmate › Uninstall**. This removes Foldmate and its web research
engine (the WSL distro `foldmate-engine`). The engine's research data is saved to a folder first. Your chats,
settings and models are kept (by default in `%LOCALAPPDATA%\PrivateLocalBot`), so installing again picks up
where you left off. Delete that folder yourself if you no longer need it.

## Known limits

- Windows 11, with a Mac preview for Apple silicon (see Mac, above).
- Foldmate isn't code-signed yet (see Install, step 2).
- Web research and OpenCode need WSL and virtualization. Without them, chat still works.
- The translations haven't been reviewed by native speakers yet.

## Help and support

- Press **F1** (or **Settings & tools › Support › Help**) for Foldmate's Help. It works offline.
- If something goes wrong, **Settings & tools › Support › Support report** shows a short summary of your PC and
  Foldmate. Read it, save it, and attach it yourself: Foldmate never sends it.
- Questions and problems: open an issue at https://github.com/griffin300/foldmate-releases/issues and choose a
  bug report, a feature request or a question about setup or models. Please don't paste chats, keys or
  passwords there; a support report already leaves them out. [SUPPORT.md](SUPPORT.md) says what to include.

## Security

Please report security problems privately, not in a public issue. [SECURITY.md](SECURITY.md) explains how.
Please don't post the details publicly until it's fixed.

## License

Foldmate is free to use but not open source: all rights reserved, under the Foldmate License that comes with
it. The open-source parts it carries keep their own licenses. They're listed in Foldmate under **App settings ›
About & updates › Open-source licenses**. To ask for the source code of the parts under the GPL, LGPL, AGPL
or MPL, open an issue at https://github.com/griffin300/foldmate-releases/issues.

Brand names and logos of the services and model makers Foldmate works with belong to their owners and only
identify those services. Foldmate isn't affiliated with or endorsed by them.
