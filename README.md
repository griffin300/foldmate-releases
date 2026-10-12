# Foldmate: friends preview (Windows)

Foldmate runs AI models on your own PC. No account.

- Your chats are encrypted on your disk.
- No telemetry.
- Web research goes through Tor by default, with no automatic direct fallback.

This is an early build shared with friends. Thanks for trying it.

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
   in the background during the first few minutes. Foldmate recommends the model that best
   fits your PC and downloads it only when you choose **Download and load**. You can pick
   another in **Models** any time.

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

## The Lens and Assist

- **Lens:** right-click Foldmate's icon by the clock and choose **Lens**, or press
  **Ctrl+Alt+Space** with nothing selected. The screen freezes. Drag a box around anything to
  ask about it.
- **Assist:** select text in any app and press **Ctrl+Alt+Space** to proofread, rewrite,
  summarize, explain or translate it with your own model.

## Known limits of this preview

- Windows only for now.
- The installer isn't code-signed yet (see step 2 above).

## Questions and problems

Tell the person who shared this with you.

Requests for the source code of the open-source parts Foldmate ships (named in its license notes,
under App settings > About & updates > Open-source licenses) go to winning1946@yahoo.com.
