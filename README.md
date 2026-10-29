# Foldmate: friends preview (Windows)

Foldmate runs AI models on your own PC. No account.

- Your chats are encrypted on your disk.
- No telemetry.
- Web research goes direct by default. Turn on Through Tor for the private route; it never falls
  back to direct.

This is an early build shared with friends. Thanks for trying it. The latest version is **1.1.2**.

## New in 1.1.2

- **Steadier computer use and PowerShell:** wide PowerShell tables are no longer cut, long command output keeps its start and end, a path built on an unset variable is pointed out, and the reply goes on when an approved step can't run.
- **Memory shared across your bots:** when the model suggests something to remember, you can keep it for every bot and mode, or only for that bot. Lens and Assist can use it too once you turn that on.
- **Automations that start on their own:** an automation can start when files arrive in a folder, with up to three of them attached, or when Foldmate starts.
- **Transcribe a window:** Ctrl+Alt+T records only the front app's sound, never your microphone, and Stop turns the recording into a transcript chat.
- **Model card settings, and fixes:** a model whose card lists recommended settings uses them by default, Deep Research quotes each page under its own link, and many smaller fixes make chats and automations more reliable. The web research service is updated too, so its first start after this update takes a little longer.

## New in 1.1.1

- **Long chats remember more:** when a long chat is compacted, Foldmate now keeps your rules and corrections word for word, lists the steps already done, and sorts what it kept, so the model forgets less. Nothing is paraphrased, and the whole chat stays saved.
- **Batch files that cmd can run:** when Foldmate writes a .bat or .cmd file that runs a path with spaces without quotes, or saves it in a form cmd can't read, it's told at once so it can fix it, instead of you finding out when the shortcut flashes and closes.
- **Safer Wallet screenshots:** a card's browser window stays blacked out while any page in it shows the shop, a card the Wallet filled stays hidden in screen text after it locks, and Show code asks for your passphrase, as Copy does.
- **More in your language, and fixes:** download messages, first-run sizes and update-check reasons are translated, first-run Retry recovers in more cases, and computer use says when a window was too slow to read in full.

## New in 1.1.0

- **Lens reads the text in a box:** Copy the text gives the words read in the box, with no model; a model that can't see pictures answers from that text, and text laid out as a table copies into Excel or Sheets. It's all read on this PC.
- **Lens blacks out personal details it recognises:** before Lens sends a picture to a cloud model, it blacks out the emails and the phone, card and Social Security numbers it recognises there. You can untick it when Lens asks to send.
- **Search the web from Lens:** Search the web opens a chat that searches about the box you drew, or about the question you typed.
- **Search the web from any app:** select text in any app, and Assist's Search the web opens a chat in Foldmate that searches about it. Emails and phone and card numbers it recognises are left out.
- **Sources under web answers:** a reply that searched the web lists its sources, numbered, and its citations link to them. Copy includes the list.
- **Recent results, and sites to skip:** in Tools & integrations, choose results from the past day, month or year for a chat, and list sites that web searches leave out (Deep research doesn't use the list yet).
- **Clearer model errors in Code:** when a cloud or Zen model stops OpenCode, the Code tab says why in plain words, such as a used-up free limit or a refused key. It no longer offers Reload last used model then.
- **Copy picture, and skip a site from its source:** Lens's Copy picture puts the box you drew on the clipboard, Esc asks before closing Lens while Do is still working, and a source under an answer has a button that skips its site in future web searches.
- **Fixes from our Lens review:** the shortcut no longer sends Ctrl+C to common terminals, a refused Lens start leaves no empty chat, photos fit in a chat, and Lens menus work from the keyboard.
- **Safer Wallet and connectors:** a card the Wallet filled guards its whole browser window, in every chat and tab, and the Wallet types a password only into a password box. A connected service's result counts as untrusted, like a web page: Always allow pauses until your next message after one (read-only tools excepted). Excel and PowerPoint use a file you already have open instead of opening it again.
- **Smoother first run and narrow windows:** Retry resumes the starter model's download, a damaged download starts over, and a full disk says so. Buttons, banners and menus fit in narrow windows and right-to-left languages.

## New in 1.0.6

- **Long tasks keep going:** when a long task fills the model's context, Foldmate sets its oldest steps aside instead of stopping. They stay in the chat's saved history.
- **More fixes from our own review:** an automation moved to another bot can't get stuck waiting for an approval, linked chats' messages get the same safety check as text read on screen, and PowerPoint gets keyboard tips.
- **Computer use:** in Full access, a command that only joins lines of text no longer asks first, and a task the model leaves half done with a stray note goes on to its next step.
- **Skills and the developer API:** fixes from a bug hunt, including clean errors instead of crashes for malformed requests.

## New in 1.0.5

- **Repeated failures stop sooner:** when a download or command keeps failing the same way, even across your approvals, Foldmate stops retrying it and tells you what went wrong.
- **Fixes from our own review:** linked chats (Resume during a running task, renaming after its chat was deleted, a full queue, a teammate named Parent), automations (Run now while an approval waits, a far-off once time, moving one to another bot) and three dialogs that screen readers now announce by name.

## New in 1.0.2

- **More fixes from our own review:** automatic deletion keeps working when one chat has many screenshots, cancelled Google pickers free up at once, Excel sheet names are checked without case, and temporary chats' uploads stay out of a bot's files.

## New in 1.0.1

- **Full access can accept licences:** in Full access, Foldmate can accept a licence agreement a task needs. In other modes it still hands the licence to you.
- **Long tasks keep their place:** on long computer-use tasks Foldmate keeps a short note of what it has done, so it finishes more of them. Scrolling to an item says when only part of a name matched.
- **13 fixes from a code review:** imports, documents, Office, Google files, voice chat, saved prompts and OpenCode behave more reliably.

## New in 1.0.0

- **Bring your chats from ChatGPT or Claude:** in **Backup & recovery**, choose your ChatGPT or Claude data export. Foldmate shows how many chats it holds, then adds them with their original dates. It's read on this PC; nothing is sent.
- **Knowledge files for a bot:** in a bot's menu, add files it reads in every chat. Replies list the passages they drew on. Only this PC's model reads them.
- **Temporary chats:** turn on **Temporary chat** in a new chat. It isn't kept, and it's deleted for good when you leave it, lock or quit.
- **Talk to your bot:** hold the microphone button to talk. Foldmate sends when you stop, reads the answer aloud, then listens again. Speech stays on this PC. Natural voices are an optional download.
- **A Wallet for your logins:** import logins from Chrome, Edge or Firefox, make strong ones, fill them with Alt + right-click or Ctrl+Alt+P, and keep two-factor codes. The model never sees the values.
- **Computer use goes further:** a task that's still making progress keeps going past 24 steps, up to 72, and Foldmate carries on after you approve a step instead of stopping to describe it.
- **Licences stay yours to accept:** a PC command that would accept a licence agreement for you is refused. The rest of the task goes on, and you get the licence to accept yourself.
- **Direct by default, Tor when you want it:** searches, downloads and connected services go direct. Turn on **Through Tor** in **Tools & integrations** for the private route; it never falls back to direct.
- **More for your chats:** archive chats, saved prompts with /, saved messages, About you for every bot, usage per day, and every chat exported in one .zip.
- **Many smaller fixes:** shorter menus, faster settings lists, translated error messages, and focus and screen-reader fixes across the app.

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
- **Faster replies:** models with built-in speculative decoding (MTP) now use it by default: faster, with the same answers.
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
- **Disk:** plan for about 15 GB free to install and set up, plus your models.
  A small model is about 1–2 GB.
- **A graphics card is optional.** Models run on the processor too, just slower.

## Updates

Foldmate checks this page for new versions directly (not through Tor, so GitHub sees your IP
address, as when you visit this page). Only releases signed with Foldmate's key install, and
each file is checked first.

When an update is available, a small arrow appears next to Foldmate's name in the sidebar.
Choose it to download the update (you can follow its progress or cancel it), then choose
**Restart to update**.

From 0.4.0 on, most updates download only the files that changed. 1.1.2 isn't one of those: its web
research service changed, so every version downloads the full installer (about 0.88 GB) to update.

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
  proofread, rewrite, summarize, explain or translate it with your own model, or search the web
  about it.
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
