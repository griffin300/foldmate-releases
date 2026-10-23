# Foldmate: friends preview (Windows)

Foldmate runs AI models on your own PC. No account.

- Your chats are encrypted on your disk.
- No telemetry.
- Web research goes through Tor by default, with no automatic direct fallback.

This is an early build shared with friends. Thanks for trying it. The latest version is **0.5.1**.

## New in 0.5.1

- **Agents:** give a bot a standing mission and a task list on the new **Team** page (in **Settings & tools**). Agents work through their tasks on their own, cloud and local side by side, and follow each chat's approval mode.
- **PowerShell that finishes the job:** long commands keep running in the background and report back, each command picks up where the last one left off, and downloads are much faster. Downloads and installs ask first, even in Full access; simple look-ups need no click in **Ask every time**.
- **Steadier computer use:** Foldmate waits for windows and dialogs to settle, switches to an app that's already open, and handles a pop-up in the middle of a task.
- **A faster first reply:** after a model loads, the start every new chat shares is read ahead, so the first chat answers sooner. Streaming replies and opening **Models** are smoother.
- **Cleaner replies:** a tool call the model writes out as text no longer shows in the chat, and the model is told when one couldn't run.
- **Fixes:** the Wallet, OpenCode Zen in projects, the context panel, pictures in chat, and keyboard and screen-reader use.

## New in 0.5.0

- **Wallet & passwords:** logins and cards are kept encrypted on this PC. The model only picks which item to use and never sees the values. Each item fills only on its own site, and purchases follow your spending limits and ask you first. Open it from **Settings & tools**.
- **A steadier Lens:** long answers no longer stop on their own, a busy model says so at once, and Do won't act on Foldmate's own window.
- **See what fills the context:** click the context ring for a breakdown by part, with **Compact now**. Compacting no longer adds notices to the chat.
- **Free cloud models in Code (optional):** OpenCode Zen's free models can be turned on per project, over Tor by default or directly. They're off until you choose them, and when on, that project's coding requests go to OpenCode Zen's servers.
- **Faster replies:** models with built-in speculative decoding (MTP) now use it by default: about twice as fast, with the same answers.
- **No Docker needed:** Foldmate's own engine runs web research and OpenCode. A PC that used Docker Desktop moves over once, automatically.
- **Many smaller fixes:** pictures in chat, computer use, keyboard and screen-reader use, and project commands in Code behave more reliably.
- **License:** Foldmate is free to use but not open source (all rights reserved). The open-source parts it carries keep their own licenses.

## Install

1. Open the **latest release** on this page and download `Foldmate-Setup-<version>.exe` under
   **Assets**.
2. Run it. Windows may say **"Windows protected your PC"**, because this preview isn't
   code-signed yet. Click **More info**, then **Run anyway**.
3. The installer sets up what Foldmate needs:
   - Microsoft's Visual C++ runtime, if your PC doesn't have it;
   - Windows' WSL, which Foldmate's private web engine runs on, if your PC doesn't have it.

   Windows may ask for permission (up to twice). A restart may be needed.
4. Foldmate opens. Its AI engine comes with it, and private web research finishes setting up
   in the background during the first few minutes. Foldmate recommends a model that fits
   your PC and downloads it only when you choose **Download and load**. Models already in
   LM Studio's or Ollama's folders show up in **Models** where they are; nothing is copied.
   You can pick another in **Models** any time.

## What you need

- **Windows 11, 64-bit.** Windows 10 hasn't been tested yet.
- **RAM:** 16 GB or more is recommended. 8 GB works with small models.
- **Virtualization turned on** in your PC's BIOS/UEFI, for web research. Without it, chat still
  works, and Foldmate tells you what to turn on.
- **Disk:** about 15 GB free to install and set up (about 9 GB stays in use), plus your models.
  A small model is about 1–2 GB.
- **A graphics card is optional.** Models run on the processor too, just slower.

## Updates

Foldmate checks this page for new versions directly (not through Tor, so GitHub sees your IP
address, as when you visit this page). Only releases signed with Foldmate's key install, and
each file is checked first.

When an update is available, a small arrow appears next to Foldmate's name in the sidebar.
Choose it to download the update (you can follow its progress or cancel it), then choose
**Restart to update**.

From 0.4.0 on, most updates download only the files that changed. 0.5.1 is one of those: from
0.5.0 it's a small download (about 15 MB). From an older version, the update downloads the full
installer (about 0.83 GB).

## Asking before it acts

Each chat has an approval mode:

- **Ask every time:** every action on your PC shows a card first.
- **Approve for me:** reading your screen, and OpenCode's work inside its project's sealed box,
  run without asking; clicks, typing, deleting and browser steps still ask.
- **Full access:** Foldmate uses your PC without asking first: it opens apps, clicks and types,
  sends and deletes, uses the clipboard, opens files and runs PC commands. Steps in protected
  windows still ask: password managers, Windows Security and Settings, sign-in and User Account
  Control prompts, Task Manager and the Registry Editor. PC commands that download or install
  software still show a card. Every action is recorded in the chat.
  Use it only in chats where you trust what the model is doing.
- **Purchases with the Wallet** ask you first in every mode. In **Wallet & passwords › Limits and
  purchases** you can allow purchases within your limits in Full access without asking (off by default).

## The tray, the Lens and Assist

- **The tray:** right-click Foldmate's icon by the clock for a small menu: **Open Foldmate**,
  **Load model** (your recent models), **Lens mode**, **Eject model**, **Settings** and **Quit Foldmate**. Quit
  unloads Foldmate's model and stops its private web research, so their memory is free again.
- **Lens:** choose **Lens mode** in that menu, press **Ctrl+Alt+Space** with nothing selected,
  or **Alt + right-click** anywhere. The screen freezes. Drag a box around anything to ask about it.
- **Assist:** select text in any app, then press **Ctrl+Alt+Space** or **Alt + right-click** it, to
  proofread, rewrite, summarize, explain or translate it with your own model.
- **Alt + right-click** is on by default from 0.4.2, even if you had turned it off. If an app
  needs that click, turn it off in **App settings › This PC**.

## Known limits of this preview

- Windows only for now.
- The installer isn't code-signed yet (see step 2 above).
- On a PC where Windows' Smart App Control is on, it may block Foldmate and its AI engine,
  because they aren't code-signed yet.

## Help

Press **F1** (or **Settings & tools › Support › Help**) for Foldmate's Help. It opens offline.
If something goes wrong, **Settings & tools › Support › Support report** shows a short summary of
your PC and Foldmate. Read it, save it, and send it yourself: Foldmate never sends it.

## Questions and problems

Tell the person who shared this with you, and attach a support report if it helps.

Requests for the source code of the open-source parts Foldmate ships (named in its license notes,
under App settings > About & updates > Open-source licenses) go to winning1946@yahoo.com.
