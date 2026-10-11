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
   - Foldmate's private web engine, which runs on Windows' own WSL.

   Windows asks for permission once. A restart may be needed.
4. Open Foldmate. On the first start, a guide points at a model that fits your PC.
   Downloading still asks first.

## What you need

- **Windows 11, 64-bit.** Windows 10 hasn't been tested yet.
- **RAM:** 16 GB or more is recommended. 8 GB works with small models. With web research
  running, the first load may say the model won't fit. Tick **Override guardrail for this load**
  to load it anyway.
- **Virtualization turned on** in your PC's BIOS/UEFI, for web research. Without it, chat still
  works, and Foldmate tells you what to turn on.
- **Disk:** a few GB for Foldmate, plus your models. A small model is about 1–2 GB.
- **A graphics card is optional.** Models run on the processor too, just slower.

## Updates

Foldmate checks this page for new versions through Tor. Only releases signed with Foldmate's key
install, and each file is checked first.

When an update is ready, a small arrow appears next to Foldmate's name in the sidebar. Choose
**Restart to update**.

## Known limits of this preview

- Windows only for now.
- The installer isn't code-signed yet (see step 2 above).

## Questions and problems

Tell the person who shared this with you.

Requests for the source code of the open-source parts Foldmate ships (named in its license notes,
under Settings > App > Open-source licenses) go to winning1946@yahoo.com.
