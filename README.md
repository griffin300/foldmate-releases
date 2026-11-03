# Foldmate (Windows, with a Mac preview)

Foldmate runs AI models on your own PC. You don't need an account, and your chats stay on your computer
unless you choose a cloud model.

- **Your chats are encrypted on your disk**, with a key protected by your Windows account.
- **No telemetry or analytics.** Foldmate doesn't report what you do, and it never sends a support report for you.
- **Models run on this PC.** A cloud model is only used when you pick one, and Foldmate asks before it sends an existing chat.
- **Web research goes direct by default.** Turn on **Through Tor** for the private route. It never falls back to direct.
- **You decide what it may do.** Each chat has an approval mode: Ask every time, Approve for me, or Full access.

The latest version is **1.1.15**.

## New in 1.1.15

- **Steadier computer use:** when a page shows Saving or Loading after a click, the assistant waits for it to finish before it looks again, and it no longer stops early on long tasks.

## New in 1.1.14

- **Your phone's view with the screen saver on:** your phone can see and control this computer while its screen saver runs, even with the display turned off. A screen saver that asks for your password still counts as locked.
- **Share control with your phone:** your phone keeps control until it hands it back. Turn on **Share control with this computer** (Remote, Advanced) to use this computer's mouse and keyboard at the same time; press Esc on this computer to take control back.
- **Smoother Remote on the same Wi-Fi:** taps and scrolling show on your phone sooner (in our tests, taps about 50 ms sooner and scrolling at about 19 frames a second instead of 15).
- **Clearer steps for you:** when the assistant needs you for a CAPTCHA, a sign-in or a card's security code, its card says what to do and where, with **Show me** and **I can't do this**. You have 15 minutes, and a step that times out is reported instead of stalling the task.
- **CAPTCHAs and checkout warnings:** **Solve CAPTCHAs for me** (Security) lets the assistant try a CAPTCHA before it hands it to you; it's on, and you can turn it off. Some sites don't allow automated CAPTCHA solving. The assistant also warns you if a shop asks for your online-banking password, and purchases still ask you first.
- **Faster first reply:** while Foldmate's web research service is still starting, your first message no longer waits for it (in our tests, about 2 s sooner).
- **Fixes:** connector labels and sign-in errors in every language, a smoother chat while replies stream, and Foldmate retries on its own if it isn't answering at startup.

## New in 1.1.13

- **A sharper, smoother phone screen:** your phone's view of this computer stays sharp while you scroll or type, moves more smoothly over Tor, and text turns crisp the moment the screen stops. Colours now match this screen. It works with the iPhone app that shows video.
- **Photos in your phone's chats:** send photos from the iPhone app to a chat on this computer's model. It needs a model that can see pictures, with Vision on. Photos go only to this computer's own model and aren't saved.
- **Safer card checkouts:** in desktop control, the model can no longer read a card's security code that you typed, and the Wallet no longer fills lists such as Country, where a near match could pick the wrong option.
- **Phone screen fixes:** with this computer's display turned off, the phone says the screen is unavailable instead of showing black, and the picture comes back as soon as the display does. After you unlock, or after Foldmate restarts, an open phone screen picks up again right away.
- **Polish:** 16 layout fixes (approval cards, the Models page, German and narrow windows), plainer wording in every language, and less background work while the window sits idle.

## New in 1.1.12

- **Foldmate for Mac (preview):** a Mac version of 1.1.12 for Apple silicon is on the same release, next to the Windows installer (see Mac, below).
- **Typing from your phone:** with the iPhone app's update, typing goes over in batches from the moment you connect.

## New in 1.1.11

- **Your phone's screen as video:** with the iPhone app's update, the phone's view of this computer streams as H.264 video, coded by Windows and decoded by the iPhone's own hardware. Videos and animations take about a quarter of the data over Tor (in our tests), and the picture adjusts to the connection so it keeps moving instead of stalling.
- **Typing that keeps up:** with the iPhone app's update, what you type on the phone goes over in batches, in order, and is never dropped for arriving late, so typing over Tor no longer falls further and further behind.
- **Better sound:** hear this computer at full quality (48 kHz stereo) on the same Wi-Fi, and much clearer over Tor: sound up to 9.6 kHz instead of about 3.6 kHz. It needs the iPhone app's update.
- **Steadier updates:** the update window keeps your place while it waits to restart, and from the next update on it shows real progress while the new version unpacks and installs.
- **Help in every language:** Help's pages about your phone and about models are now fully translated.
- **Fixes:** model settings no longer say a setting changed when none did, the welcome card keeps its newer design after you choose a different model, Test this computer no longer offers a graphics-card engine on a PC without one, and many smaller fixes.

## New in 1.1.10

- **Send email from Gmail:** connect Gmail in Connections, then ask in any chat to email someone, as with Outlook. You see the whole email, and can edit it, before it goes. Foldmate can send mail but never read it. Until Google finishes reviewing Foldmate, Google's sign-in page warns that it hasn't verified the app, and at most 100 people can connect Gmail.
- **Foldmate in your language:** every screen and help page is now in Arabic, Chinese, French, German, Italian, Japanese, Korean, Portuguese, Russian and Spanish. The translations were made with AI help and haven't been reviewed by native speakers yet, so corrections are welcome on the Issues page.
- **A calmer look:** a reply's copy, branch and other buttons stay out of sight until you point at the reply, and the tray menu has a quiet border and lines up like other Windows menus.
- **Clearer messages when something goes wrong:** if setup, web research or a model can't start, Foldmate says what happened and what to do next, with the technical details a click away.
- **Hear your computer on your phone:** with the iPhone app's update, tap the speaker while you watch the screen to hear this computer's sound. This computer shows when a phone is listening.
- **Sharper and smoother on the same Wi-Fi:** on this computer's Wi-Fi the phone's picture is clearer and scrolls more smoothly (in our tests 8.8 updates a second instead of 8.1 at the Normal size), and Sharper goes up to 1920 pixels wide.
- **Smoother typing over Tor:** over Tor, the phone's view of this computer updates about twice as often while you type (in our tests on real Tor, 4.8 times a second instead of 2.7), at the same picture quality.
- **Drag anything from your phone:** dragging a tab or a window from the phone no longer stops halfway. Foldmate no longer second-guesses your own taps: only Windows can block one, and the phone says why.
- **Approve more from your phone:** a phone allowed to approve actions can now approve PC commands and coding steps too. Wallet cards still need the computer.
- **Simpler phone pairing:** pairing shows one request at a time, named for the phone, and closes by itself when it's done. Your phone says it was declined only when you press Deny.
- **Fixes:** an email to an address you didn't type in the chat is approved on the computer, the phone can lock this computer with Win+L, and many smaller fixes.


Older versions' notes are on the [Releases](https://github.com/griffin300/foldmate-releases/releases) page.

## Install

1. Open the **latest release** on this page and download `Foldmate-Setup-1.1.15.exe` under **Assets**.
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

The Mac preview is version 1.1.12: download `Foldmate-1.1.12-mac.dmg` under **Assets** on this release. It's built
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

From 0.4.0 on, most updates download only the files that changed. 1.1.15 is one of those: from 1.1.14, 1.1.13 or 1.1.12 it's a small download (about 19 MB). From an older version,
the update downloads the full installer (about 0.88 GB).

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
- Questions and problems: open an issue at https://github.com/griffin300/foldmate-releases/issues. Please
  don't paste chats, keys or passwords there; a support report already leaves them out.

## Security

To report a security problem, open an issue that says only that you have one to report, with no details, and
we'll arrange a private way to send it. Please don't post the details publicly until it's fixed.

## License

Foldmate is free to use but not open source: all rights reserved, under the Foldmate License that comes with
it. The open-source parts it carries keep their own licenses. They're listed in Foldmate under **App settings ›
About & updates › Open-source licenses**. To ask for the source code of the parts under the GPL, LGPL, AGPL
or MPL, open an issue at https://github.com/griffin300/foldmate-releases/issues.

Brand names and logos of the services and model makers Foldmate works with belong to their owners and only
identify those services. Foldmate isn't affiliated with or endorsed by them.
