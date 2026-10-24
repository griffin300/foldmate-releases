# Foldmate: friends preview (Windows)

Foldmate runs AI models on your own PC. No account.

- Your chats are encrypted on your disk.
- No telemetry.
- Web research goes through Tor by default, with no automatic direct fallback.

This is an early build shared with friends. Thanks for trying it. The latest version is **0.6.2**.

## New in 0.6.2

- **Agent teams:** start a Researcher, Writer and Reviewer team under any chat in one step. The **Team** board shows what each linked chat is doing, what waits and its last result.
- **Agents ask when they're stuck:** a linked chat that needs something only you can do tells you in its parent chat, with **Open its chat**. A declined approval no longer leaves it waiting.
- **A daily brief:** **Automations** has a **Daily brief**: each morning, what your agents finished, what's waiting for you and what's still running, from this PC's model.
- **Read further in a referenced chat:** when you reference another chat in a message, Foldmate can search and read more of it for that message.
- **Computer use keeps going:** many steps at once no longer end a turn, Foldmate carries on when it says what it will do next, and it hands you a step only after looking at the screen.
- **OpenCode effort per project:** choose OpenCode's effort in the Code model menu. Code also shows when OpenCode compacts a long session.
- **Fixes:** **Rules** lists every Always allowed tool, chat notices are translated, and agents, automations and screen readers work more reliably.

## New in 0.6.1

- **One menu for Code's model:** the model button in Code lists this PC's models, OpenCode Zen's free models and your cloud models, and shows which one each chat uses. **/model** opens the same menu.
- **Free Zen models that work:** turning on OpenCode Zen in a project that already has chats now works, and the menu offers Zen's current top three free models, those that keep no data first, each with what its provider keeps. Without a connection, the menu says so and keeps the last list.
- **Computer use finds the right item:** Foldmate scrolls a long list until the item you named shows, won't act on a similar-looking row by mistake, and notices changes it can only see in the screenshot.
- **Undo a memory change:** a bot's memory shows how full it is, and **Undo** puts back its last change for a day.
- **Bring another chat in:** drag a chat from the sidebar onto the message box to reference it in your next message.
- **Every rule in one place:** **Blocked commands** also lists the rules Foldmate always follows.
- **Fixes:** chats kept on disk, decision models, OpenCode sessions, the model picker and OpenCode's questions behave more reliably, and every language is complete again.

## New in 0.6.0

- **Linked chats:** start a chat linked to this one, on its own model: this PC's, a cloud model, or a free Zen model in Code. The two message each other, and **Open side by side** shows both.
- **One model per Code chat:** type **/model** to give each Code chat its own model, local or a free OpenCode Zen one. Switching a chat to Zen, and attaching a file in a Zen chat, ask first.
- **Code tasks told in a few lines:** a longer Code task is summed up as it works (what it read, changed and ran), and folds back to that summary when it finishes.
- **Steadier computer use:** Foldmate sees each control's state (on or off, expanded, how far a list is scrolled), can search a long window past what one look shows, says whether an action changed the window, stops when a dialog opens over it and stops repeating a step that isn't working. If Send, Pay or Delete shows no change, it isn't pressed again: Foldmate tells you it may have gone through.
- **Answer OpenCode's questions:** when OpenCode needs a choice, it asks in the chat. Pick an answer, type your own or skip.
- **This PC's model can approve routine steps (optional):** in **Approve for me**, a switch lets your own model approve a step that's clearly what you asked for. Passwords, payments, protected windows, downloads, risky commands and deleting always ask you. It's off until you turn it on.
- **Vision on the GPU or the CPU:** when loading a model, choose where its vision part runs. On the CPU the graphics card stays free for the model itself, and pictures take longer to read.
- **Pictures from connected services** go to this PC's vision model only, never to a cloud model.
- **Keep chats ready on disk (optional):** in **Settings**, an encrypted working copy of recent chats makes switching back faster after the engine restarts.
- **Your data, in one place:** storage, backups, the Wallet, cookies and Trash share one popup. **Blocked commands** are refused in every mode, Full access too.
- **Fixes:** shorter tool descriptions leave more room for your chat, and connected services, Zen in Code and pictures in chat behave more reliably.

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

From 0.4.0 on, most updates download only the files that changed. 0.6.2 is one of those: from
0.6.1 or 0.6.0 it's a small download (about 17 MB). From an older version, the update downloads the
full installer (about 0.88 GB).

## Asking before it acts

Each chat has an approval mode:

- **Ask every time:** every action on your PC shows a card first.
- **Approve for me:** reading your screen, and OpenCode's work inside its project's sealed box,
  run without asking; clicks, typing, deleting and browser steps still ask. An optional switch
  (off by default) lets this PC's model approve routine steps that are clearly what you asked for.
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
