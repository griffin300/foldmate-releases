# Foldmate (Windows, with a Mac preview)

Foldmate runs AI models on your own PC. You don't need an account, and your chats stay on your computer
unless you choose a cloud model.

- **Your chats are encrypted on your disk**, with a key protected by your Windows account.
- **No telemetry or analytics.** Foldmate doesn't report what you do, and it never sends a support report for you.
- **Models run on this PC.** A cloud model is only used when you pick one, and Foldmate asks before it sends an existing chat.
- **Web research goes direct by default.** Turn on **Through Tor** for the private route. It never falls back to direct.
- **You decide what it may do.** Each chat has an approval mode: Ask every time, Approve for me, or Full access.

The latest version is **1.1.35**.

## New in 1.1.35

- If no picture model is on this PC, asking for a picture in a chat offers one to download, picked for this PC, with its size. When it's installed, Make the picture uses your request.
- Copy and Edit on a draft are icons now, and its bar turns see-through while text scrolls under it, so you can keep reading.
- Notes now sits in the options menu, and Your data and memory is called Data & memory. In App settings > This computer you can turn on a shortcut that opens Notes from anywhere; it's off until you choose one.
- Strata now prepares its MTP draft layer for Q2_0 models too. If the layer can't be prepared, the Load sheet says why and offers Retry, and the model loads without it.
- The Load sheet and the launch now use one memory check that counts the context you chose, so Strata no longer falls back to disk mode on a PC that has room.
- The Load sheet's GPU memory reserve now applies to Strata too, so the desktop and other apps keep some video memory.
- Direct search skips engines that stopped answering, adds Mwmbl, and waits at most 3 seconds for any one engine.
- When you choose to restart after a reply finishes, Foldmate now waits for all running work, a second request no longer cancels the wait, and a failed restart says so instead of showing Ready.
- Turning off the phone's microphone permission drops a clip still on its way, and muting the phone in one chat no longer leaves another chat's phone muted.

## New in 1.1.34

- Ask for a picture in a chat and Foldmate makes it with picture models you added (My models or a Hugging Face download), not only the catalog's. A cloud picture model you set up counts too. Before, chat could say it had no picture tool.
- If a reply or task is still running when you choose Restart to update, the update window asks: restart anyway, or when it finishes. No Windows box that can hide behind Foldmate.
- An update you already downloaded is ready when you open Foldmate again, instead of downloading a second time. If its file is in use or the drive is full, Foldmate says so.
- When Windows has too little memory left for Strata's fast mode, the model now reads its experts from disk instead of failing to start.
- Foldmate now clears the icons that earlier runs or an interrupted update left in the notification area, so only one stays.
- If saving a storyboard, an Audio Studio project or a video edit fails, your changes stay and Foldmate says why. Delete in Audio Studio names the project it removes.
- With Strata as the backend, choose MTP under Speculative decoding when you load a model. Strata downloads a 0.9 GB draft layer once and then writes faster. If MTP doesn't start, Strata loads without it.

## New in 1.1.33

- Faster web search: Direct search no longer waits on engines that never answer, and a search for a timer or a tool keeps fewer pages that only share a few letters with it. Through Tor, each site's rules are read ahead, so a typical search finishes about 9 seconds sooner.

## New in 1.1.32

- Fusion: a cloud model you set up and this PC's model can work together in a chat or a Code project, either one leading. It stays off until you turn it on, with a cap on cloud tokens.
- Chat bar replies show bold, lists, tables and code cards, each with its own Copy. The context panel splits the window part by part, and Context shows what compaction kept.
- Long tasks on this PC hold together: when a task outgrows the context, old screen readings go first and your request and the model's notes stay, so it keeps its place and finishes much sooner.
- The Wallet opens with Windows Hello or a recovery key, both off until you set them up. Lock an Imagine folder to keep its files encrypted and hidden, or lock a Code conversation.
- With Direct browsing, the browser panel is a real browser inside Foldmate's window, with tabs. It never reaches this PC's own addresses or your home network. Tor browsing stays in the private browser.
- Model search keeps drafters and helper files apart from chat models, shows more results and GGUF builds, and opens pasted links. Code has a Local only switch; its web search and MCP go through Tor.
- Chat and connected agents use the picture model you choose, in Imagine's model menu or in Tools. Chat can ask for a size, a tileable texture or a negative prompt, and says plainly when a model is missing or too big for this PC.
- Imagine makes material maps, game engine packs and pixel art, and its MCP server makes sounds and sprite sheets. Turn on Make assets in Code's Tools menu and OpenCode saves pictures and sounds in your project.
- With Keep the private link on, a dropped phone link tries again by itself. No total quota on your pictures and documents, only a free-disk floor. A failed load offers Load without Vision.

## New in 1.1.31

- Animation editor (first version) in Imagine: layers, keyframes with easing and a graph editor, parenting and null layers, bones that reach for a target, puppet pins, onion skin and autosave.
- Pipelines has a workbench around the canvas: library tabs, an inspector, a dock with each run's times and log, lining up, find, and a list of recent runs.
- My models takes your own text encoders, VAEs and audio models, and reads folders you add, such as a ComfyUI models folder. Each model says what it still needs.
- Seamless textures: make a picture that tiles edge to edge, check it with Tile preview, and upscale it to 4096 x 4096. Claude Code can ask for textures through Imagine's MCP server.
- The model loading screen is slimmer: one summary card instead of five, and Loading settings are open from the start.
- Computer use: when a chat has thinking on, steps on your PC now think at a lighter level of their own, so a task finishes much sooner.
- Code tab: type @ and a file's name to hand it to OpenCode, and send the terminal's output with your message. The context ring shows when OpenCode will compact.
- Wallet: sites and cards show their brand's mark, bundled with the app and never fetched, and a card's row says when it expires. Foldmate's own PC commands are refused if they name the Wallet's files.
- Same Wi-Fi connection for the phone adds one Windows Firewall rule when you allow it, so Windows no longer asks after an update. Imagine uses the slim scrollbar everywhere. Cloud models stay off unless you turn them on.

## New in 1.1.30

- Pipelines is now a node canvas: connect picture, video, sound, text and logic steps, run them through Imagine's queue, and start from ready-made starters that end in a finished picture, clip or video.
- My models: put a .gguf or .safetensors picture or video model file in the My models folder and it shows up in Imagine, ready to use. Foldmate reads what it is from the file, and you can set its steps, CFG and sampler.
- Code tab: a terminal for your own commands in the project folder, in a dock under the conversation that can pop out into its own window. Files and Changes are icon buttons, and the approval card's note is one line.
- Video editor: ripple, roll and slip trims, keyframes, speed ramps, cross dissolves, adjustment layers, captions that light up each word, voiceover at the playhead and YouTube export presets.
- Audio Studio: stem split, transcripts that edit the audio, Reverb and Delay sends, punch-in recording, clip gain and Normalize, loudness on export, and FLAC and MP3 files.
- Image editor: adjustment layers and filters, free transform, quick mask, pen pressure, AI edits that land as a layer, Select subject and Remove background on this PC. Selection outlines are smooth lines that march gently.
- AI fill, Expand, Remove, Vary, Enhance, Draw and Characters work with the model that Get started installs. A custom picture size can go up to 2048 px a side and about 2.4 megapixels, depending on your graphics memory.
- Video from words alone: this PC makes the first frame, then animates it, in a wide, tall or square shape. A 4-step Wan 2.2 Turbo model is in the catalog as an option, under a non-commercial licence.
- Chat and Code got a polish pass, Eject stays clickable at every window size, saving to the gallery and voice cloning answer again, and a run that runs out of memory says so. Cloud models stay off unless you turn them on.

## New in 1.1.29

- Your own browser in the side panel: tabs, an address bar, Back and Forward. Click and type right in the page. Sites you sign in to stay signed in, and that data is kept encrypted on this PC.
- The AI can use this browser only when you say so, and a strip with Stop shows while it does. Direct is the default route. Tor is one click, and changing the route opens a new browser.
- Pictures: up to 16 in a message, each up to 32 MB. They are kept up to 2560 pixels on the long side by default, and you can raise that to 4096.
- The model sheet is much shorter on the Load and Inference tabs, with less text and a smaller chart. The context panel shows a labelled breakdown, including the system prompt and tools.
- Imagine shows a small loaded-model bar with an eject button. The plus next to Pictures brings images from your PC into the image editor.
- The video editor can clone a voice or use a saved one from its AI tools and make speech for your video.
- Browser, Activity and Split view are now simple icons at the top right. Add files opens the picker at once, and Transcribe audio has its own row in the + menu.
- The Build and Plan switch slides between modes. The Code tab no longer warns that OpenCode cannot start before you have used it. Chat redraws less while a reply streams and while the app is idle.
- Your browser sign-ins stay encrypted on this PC. Cloud models stay off unless you turn them on.

## New in 1.1.28

- **Unsaved work stays safe:** switching projects or starting a new one in Audio Studio saves first and asks before discarding anything. An older video project file can no longer replace a newer one, and renaming a picture counts as a change.
- **Late replies land where they belong:** an AI picture edit, captions, an export start or a saved voice that arrives after you moved on no longer lands in another picture, timeline or mode. **Stop** always stops an image AI edit.
- **Video editor fixes:** **Close** and **Discard changes** close the editor with a picture clip on the timeline, the image and video switch works after discarding, and an untouched project no longer asks about unsaved changes.
- **Steadier video agent:** **Speed** fits the clip to its source like the Speed control, a title goes after the titles already there and one Undo removes it, and every step acts on the clip chosen when the plan ran.
- **Small windows:** the video editor keeps Project media beside the inspector. Space on a focused button presses it, and chapters past the end of the timeline are flagged before you copy them.
- **Chat opens with your bot:** not the bot of your last Code session. The update card can be closed and no longer stays on top of other windows.
- **Gallery and Library:** the Library shows JPEG pictures. The gallery no longer lists sounds, and Audio Studio opens with the example voices on its tracks.
- **More fixes:** Esc that closes the model browser no longer also asks to close the editor, the Create panel stays closed after a restart, and the image agent leaves a locked layer alone.

## New in 1.1.27

- **AI edits in the image editor:** describe a change on the **AI tools** tab and it's made on this PC. Select a part first and only that part changes. The result arrives as a new layer, so you can hide or undo it.
- **Agent in the editors:** tell the agent what you want, like warmer colours, a 4:5 crop and a title. It plans the steps with your chat model, you check them, and each one runs as an undoable edit. In the image and video editors.
- **Pick the AI models:** the **AI tools** tab in both editors shows which picture or video model makes the change, and which chat model the agent plans with. Switch either one there.
- **Image and video editor switch:** the icons by the editor's title switch between the image and video editors. The picture goes with you.
- **A better magic wand:** the magic wand has its own place in the tools. Set **Tolerance** in percent and the selection follows as you drag. It has smooth edges and a mode that inverts where selections overlap.
- **Smoother zoom and pan:** zoom glides instead of jumping, and a flick of the hand tool keeps moving a little. **Reset tools** puts every tool back as it started.
- **YouTube tools in the video editor:** J, K and L for playback, markers you can copy as YouTube chapters, punch-in zoom, close gaps, 4K and Shorts frames, and a 1280 x 720 thumbnail export.
- **Captions on the timeline:** make captions from a clip's speech, on this PC. They land on their own track, one line at a time.
- **Title templates and styles:** name and role, subscribe reminder, chapter card and end screen templates. Give any title an outline, a shadow or a box so it reads on any footage.
- **Clearer waveforms and smoother knobs:** waveforms in Audio Studio and the video editor fill their clips and show every syllable. Knobs turn smoothly with a drag up or down, Shift for fine control.
- **Voice tools in Audio Studio:** **Clone a voice** or **Use a saved voice** from AI tools. **Clean up voice** and **Remove noise** work on your speech track without picking a clip first.
- **Example voices:** if your gallery has no sounds yet, it shows four example voice clips, each with the words and voice that made it. Delete them like any item.
- **Close the Create panel:** close the Create panel in any Imagine view for more room. A small icon brings it back.
- **More fixes:** late replies no longer land in the wrong project, the image editor's toolbar fits at common window sizes, batch and queue controls keep your place, and video exports retry a dropped connection.

## New in 1.1.26

- **Video exports save again:** **Export to gallery** in the video editor saves the clip again. In 1.1.25 it stopped at Saving and the clip was lost.
- **Titles in video exports:** video editor exports with a title work again. In 1.1.25 they were refused with a message about drawing titles.
- **H.264 and AAC exports:** the video editor exports H.264 video as MP4 or MOV, and AAC audio as M4A, with Windows' own encoders.
- **Video editor fixes:** animated size and opacity export as they play in the preview, a split clip keeps its animation, trims stop where the clip's video starts, and **Solo** only quiets other sound tracks.
- **Layer styles:** give any layer in the image editor a drop shadow, an outer glow or an outline, with its own color and size. Rasterizing a layer keeps its style.
- **LUTs in Adjust:** import a 3D LUT (.cube) from Lightroom, Premiere, Resolve or a film pack on the **Looks** tab and set how strongly it applies, or export your look as a LUT for those apps.
- **Split at scene changes:** in the video editor, split a clip at each change of shot in one step. It runs on this PC.
- **Piano roll in Audio Studio:** write notes for a built-in synth or drum kit in a key and scale, let the note tools write chords, an arpeggio, a bass line, a melody or a beat, bring MIDI files in and out, and add the pattern to your tracks. The pattern is saved with the project.
- **Smoother Imagine gallery:** scrolling a long gallery, opening a picture's details and moving between chat and Imagine no longer stall or redraw the gallery on a slower PC.
- **Redesigned video editor:** Project media with search and filters, film strips and detailed waveforms on the timeline, workspaces across the top, and Clip, Audio, Effects and Color in the inspector. One click brings a clip onto the timeline, and Export is no longer under the window's buttons.
- **Redesigned image editor:** the image editor and Adjust are one window: your pictures to add as layers, a column of tools, Layers, Adjust, Effects and AI tools on the right, and Generate, Expand, Remove and Improve across the top. **Edit** beside Image or Video opens the editor, and videos have **Edit** in their details.
- **Retouch and selection tools:** the image editor has a **magic wand**, Shift and Alt to add to or take away from a selection, **Select > Modify** (Feather, Expand, Contract, Border), and new brushes: spot healing and healing (they take the light around the spot), blur, sharpen, smudge, **Liquify** (push, bloat, pucker, twirl; also Filter > Liquify), dodge, burn and sponge. Right-click a tool, or press and hold it, for the others in its group.
- **Distort and Perspective:** **Layer > Distort** and **Layer > Perspective** in the image editor drag a picture layer's corners, with a live preview; Enter makes the pixels at the layer's own resolution, Esc cancels.
- **Saturation, Chorus and Delay:** Audio Studio tracks have three more effects in their chain and the Effects Rack. The Delay follows the project's tempo (1/4, 1/8, dotted 1/8 or 1/16 note).
- **Turn and flip video clips:** Transform in the video editor turns a clip to any angle and flips it, in the preview and the export.
- **Green screen:** **Effects > Chroma key** in the video editor removes a green or blue screen, or a colour you pick, with Similarity and Smoothness, so the tracks below show through.
- **Engine filter on Hugging Face:** Works with Foldmate's engine now finds the image and Wan video models the engine runs.
- **Clearer Imagine bar:** the top bar shows each button's name. **Edit** on a picture opens the full image editor; the AI's edit by instruction is now **AI edit**.
- **One-click screenshots in the chat bar:** the chat bar's screenshot button takes the whole screen at once, with no strip to draw a box in, and the chip says **Your screen**. A chat bar left open no longer closes on its own ("This bar has closed") after ten minutes.
- **Chat bar opens sooner:** the chat bar no longer waits for a slow app to say what's selected. The selection follows a moment later.
- **Big model engine:** with a recent NVIDIA or AMD card and enough memory, Qwen3.8-Flash-Next can run on Strata, an optional engine you install in one click from **Models**. On a test RTX 4080 it answered 1.4 to 2 times as fast as the standard engine. The model is under the Qwen Community License 1.0.
- **Image editor fixes:** color changes undo in one step and Cancel leaves no trace, an open adjustment holds the rest of the editor, a duplicated group keeps its pictures, and a crop or turn in Adjust keeps its shape.
- **Saves keep your latest edits:** edits made while a save or export runs are kept, in Audio Studio, the video and image editors, Storyboard, notebooks and model presets. **Remove canvas** removes the canvas on screen.
- **Approvals in the chat bar:** a small shield beside **Tools** shows the chat's approval mode and changes it, as in the main chat. Cards in the bar offer their real answers, and anything the bar can't show opens in Foldmate.
- **Redesigned model loader:** **Load** and **Inference** are compact cards: a memory timeline, this PC's tightest resource, a compatibility check, the main loading settings with the big model engine switch in view, sampling presets, and your system prompt beside them. Every setting is still there.
- **Clearer model downloads:** in the model browser, **Quantization** is a table: each version's size, what it is for, whether it fits your GPU and its own download button, with **Download selected** under it.
- **Imagine beside your chat model:** when there's room, Imagine makes pictures with part of its model in system memory instead of unloading your chat model. When it does have to unload it, the chat model loads again by itself after the pictures are done.
- **More fixes:** a clip can't run past the end of its video, a layer's mask turns with the layer, and text typed in the image editor is kept when you click away.

## New in 1.1.25

- **A full image editor:** **Adjust** gains brush masks and masks by brightness or a picked color. Switch it to **Layers** for layers and masks, selections, brushes, clone, fill and gradients, text, shapes and the pen, curves, levels and more adjustments with a live preview, and a full history.
- **A video editor:** cut gallery clips on a timeline with video, title and audio tracks: the blade, snapping, fades and transitions, keyframes for position, size and opacity, and export to MP4 (AV1), WebM, MKV, GIF and more.
- **Audio Studio, rebuilt:** tracks hold many clips. Split them, regenerate one into alternate takes, draw volume and pan lines, duck music under a voice, and work in **Arrange**, **Mix** or **Master**. Projects save on this PC, and the side panel folds away to give the tracks room.
- **Captions for any video:** make captions for a gallery video with speech-to-text on this PC, edit and time each line, choose a look, then draw them into the video or save an SRT file.
- **Reframe:** turn any gallery video into 9:16, 1:1, 4:5 or 16:9, held still or panning.
- **Clean up, smooth and tighten:** **Clean up voice** lowers hiss, hum and room noise, **Smooth motion** makes a clip 60 fps or slow motion, and **Cut the pauses** shortens the silences between sentences. All three also work from the phone.
- **Imagine's top bar:** Imagine's sections move to a bar across the top, the model browser and Library are redone, and Characters Workflows and the Storyboard follow the new look.
- **Characters in a cloned voice:** a character can speak in a voice cloned on this PC. The first time, Foldmate asks you to confirm you may use that voice.
- **A faster start:** Foldmate's window appears at once and finishes loading while the rest of the app starts.
- **Better on NVIDIA cards:** the first chat model loads on the CUDA engine when it's installed, FLUX.2 klein stays on 16 GB cards and runs faster, and a missing CUDA runtime is named instead of asking you to update the driver.
- **Claude Code and Codex:** the MCP window has setup tabs for Claude Code and Codex.
- **Fixes:** the Qwen3.8 27B pick for 16 GB cards loads with the Q4 cache its note asks for, and Imagine's page no longer scrolls under its top bar.

## New in 1.1.24

- **Agent as a director:** pick a workflow such as an ad, a short film or a social clip, write the brief, choose pictures, video, sound and **Edit**, and **Run Agent** plans the steps, makes them and puts the clips and the sound together into one video.
- **Imagine pipelines:** build a pipeline of up to 12 steps, each with any installed model and its own Advanced settings. One run makes up to 48 jobs.
- **Characters in their own window:** Imagine's Characters open in a window: a library of people, mascots and products, with their reference pictures, poses, voices, clips and export packs.
- **MCP window:** set up Claude Desktop, Cursor, OpenCode, Windsurf or VS Code to use Foldmate, see each agent's permissions, and revoke one.
- **Pictures in Image mode:** Image mode has **Add a picture** for models that use reference pictures, such as FLUX.2 klein.
- **Hugging Face installs:** install an image or video model from Hugging Face in any family Foldmate recognises, not only SDXL. SD 3.5 is still not supported.
- **Audio Studio mastering:** the Audio tab is laid out for mixing and mastering: a five-band EQ with a draggable curve, a compressor, reverb and a limiter. Export writes 16- or 24-bit WAV at 44.1 or 48 kHz.
- **Settings in six sections:** and **Keep the private link on** starts the link with Foldmate when Tor is installed and lockdown is off.
- **Imagine on the phone:** install Imagine models from a paired phone. Newly paired phones have Imagine on by default.
- **Plainer names:** Assist and Lens are gone from the app's words: the chat bar is the **Chat bar**, Ctrl+Alt+Space is the **Selected text** shortcut for **Quick actions**, and voice mode's characters are now **Companions**.
- **Fixes:** Explore previews load again, Fits my GPU shows your card's real size, the Imagine feed bar wraps when the feed is narrow, and voice, character and photo-preset bugs are fixed.

## New in 1.1.23

- **Voice mode:** **+ > Voice mode** opens its own window: a live transcript, push to talk or hands-free, interrupt anytime, and your choice of microphone and voice.
- **Characters:** characters have cards with portraits. Add one of eight starters or make your own with a picture, a persona, a greeting and a voice. Your paired iPhone can use them too.
- **Characters that can use tools:** turn on a character's **Web research and PC control** switch and it can search the web and use your PC. It's off by default, and your approval settings apply.
- **More photo tools:** **Adjust** adds Heal, Color grading, Noise reduction, Dehaze and Perspective, a before and after view, and presets of your own settings.
- **A fuller audio studio:** tracks can play backwards, faster or slower, through a tone and with an echo. Snap clips to the beat, master with a preset and save each track on its own.
- **Start and end frames:** cloud video can start from your picture and end on another with Kling, Veo 3.1, Wan 3.0, Seedance, LTX 2.5 and MiniMax H3 Max.
- **More video models:** eight more video models install on this PC, including Wan 2.1 1.3B for 8 GB cards and smaller MiniMax H3 files, and video can start from words alone. New with your own fal key: FLUX 3 video, LTX 2.5 fast, Wan 3.0 prime and MiniMax H3 Max. MiniMax H3's licence excludes some regions: its card shows the terms.
- **Camera moves:** video can ask for a camera move: push in, pull back, pan, orbit, crane up, handheld or locked off.
- **Search all models:** one search finds this PC's models and the cloud's, every kind at once.
- **Speak with your fal key:** Speak can lip-sync a portrait or a face video through fal with your own key.
- **More Imagine on the phone:** on the phone page's **Imagine** tab, make videos and sounds too, pick the model and style, save to the phone, or move a picture to the PC's Recycle Bin.
- **Updates while you work:** a full update installs while you keep working. Foldmate closes only at the end.
- **A calmer chat bar:** the microphone button and the status line left the chat bar. **Dictate** and **Voice mode** are in the **+** menu, and Ctrl+Shift+Space still dictates.
- **Fixes:** photo edits made after or during a save ask before they're lost. Leaving Audio stops a recording. Play works after a seek and plays the clip you chose. A failed voice save can be tried again.

## New in 1.1.22

- **An audio studio:** Audio is a studio now. Play clips together as tracks, place, trim and fade each one, record from your microphone, master the mix with EQ, compressor, reverb and limiter, and save it to your gallery.
- **Voice cloning:** make a voice from a short clip of someone who agreed to it, then speak any text in that voice, on this PC. Each voice keeps your confirmation. The two voice models install on this PC (about 3 GB each).
- **Characters:** **+ > Voice mode > Characters**: give a character a persona and a voice, then **Talk** to it out loud. Its replies are read in its voice when the Natural voice is installed.
- **Adjust your pictures:** **Adjust** on any picture: light, color, a tone curve and color mixer, detail, vignette and grain, crop and straighten, looks and **Auto**. It saves a new picture and keeps the original.
- **Text on pictures:** in **Adjust**, add text to a picture, drag it into place, and choose its font, size, color and shadow.
- **Imagine from any phone:** the phone page has an **Imagine** tab: describe a picture, pick its shape and make it on this PC, watch it run, and browse your gallery. It needs the phone's Imagine permission, which is off until you turn it on in **Remote**.
- **A quicker start:** Foldmate's window keeps its own scripts between starts instead of loading them all again.
- **A quicker chat bar:** over apps that don't share their selection, the chat bar opens without waiting for a copy. Text you selected still joins the bar when it arrives.
- **Fixes:** a bot's notebook edit no longer overwrites a page you saved meanwhile, and code examples in pages are no longer read as sections. Phone camera photos are taken only over your Wi-Fi. Imagine's view buttons are centered.

## New in 1.1.21

- **Notebooks:** attach a folder of Markdown pages or your Obsidian vault to a chat. The bot reads and searches it, and its edits come as suggestions you accept, or apply with Undo. Pages stay in their folder on this PC.
- **Pictures from the chat bar:** type what you want and choose **Make a picture**, or **Make a picture from this** to start from your screen. **Change the last picture** makes a new version from your words.
- **Pictures in Chat:** in a chat, the model can make a picture on this PC when a picture model is installed. Before it frees graphics memory, it asks you once.
- **Your phone's camera in Imagine:** **Phone camera** asks your paired iPhone for a photo to start from. It travels over your own Wi-Fi only and lands on this PC as the phone took it. It needs the Foldmate iPhone app and the same Wi-Fi connection turned on in Remote.
- **Imagine from your iPhone:** the Foldmate iPhone app can make pictures and clips on this PC and edit them. Each phone needs its Imagine permission, which is off until you turn it on in Remote.
- **Notes in Settings:** Settings > Notes lists your notebooks and quick notes: add a folder or an Obsidian vault, rename, choose the default, export.
- **Example pictures:** an empty Imagine gallery starts with example pictures, each with its model, settings and prompt. Delete them like any picture.
- **Picks for this PC:** **Get started** opens a **For this PC** tab with image, video and audio models that fit this PC's graphics memory.
- **More cloud models:** cloud providers show as cards with their logos, and 12 more image, edit and video models come through fal with your own key.
- **A tidier Imagine:** a wider Create column you can resize, the tools in one row, a button to bring back a hidden sidebar, a Close bar in picture details, and a menu on each picture's ⋯.
- **Phones reconnect on their own:** if the phone connection can't start, Foldmate tries again every 20 seconds, and Remote shows why with a **Retry** button.
- **Fixes:** NVIDIA PCs fall back to the standard engine when the CUDA one can't download. FLUX.2 klein 4B, Z-Image Turbo and Chroma1-HD install again. A rare freeze when moving a chat from the chat bar is gone.

## New in 1.1.20

- **Imagine, redesigned:** a Create column, a results bar for Generations, Queue and Pipelines, and an inspector for each picture.
- **Start from a picture:** Image mode can start from a picture you add or one you made. Choose how much it may change; the shape follows the picture. **Start from this** in a picture's details puts it there.
- **Speech, music and sound effects:** Imagine has tabs for each. Each model installs on this PC with one click. Each model shows its licence in the catalog.
- **Agent as a director:** the Agent tab turns a description into a plan with steps and prompts. You can check the plan before you run it.
- **Makers' logos:** model cards and Hugging Face results show each maker's logo where the maker has one. Rebel AI quants say so on their cards.
- **Provider logos:** the model picker shows a provider's logo on each cloud row. Custom providers show their host's logo where one is bundled, and a plain cloud otherwise.
- **Start in a new folder (Code):** makes an empty folder in Documents\Foldmate and opens it as a project. The folder is made only when you click.
- **Made files:** each made file says what kind of file it is, such as Word document.
- **Reviewed marks (Code):** the marks in the Changes panel stay after a reload or restart.
- **Scheduled Code tasks:** an automation can run a task in a Code project on a schedule, such as Mondays at 10:00: run the tests and summarize failures. Each run is a new Code conversation in Plan; it only reads and runs the commands you list.
- **Trace:** a conversation's ⋯ menu opens Trace: how long each turn took, where the time went, and every tool call with its arguments and result. Export only when you click it.
- **Show progress:** Settings > Chats chooses just results, key steps or everything. It changes only the display.
- **Glass style:** dropdowns, checkboxes and radio buttons share one style.
- **Beta updates:** Settings > Advanced has a switch to receive beta updates. It is off unless you turn it on.
- **Installer:** opens in one window with the Foldmate mark, its name and one status line.

## New in 1.1.19

- **Imagine, rebuilt:** a clearer Models sheet that suggests models for this PC, six shortcuts in the sidebar, and **This PC** or **Cloud** on every model. Imagine no longer uses ComfyUI.
- **Civitai checkpoints on this PC:** install SD 1.5, SDXL, Pony and Illustrious checkpoints from Explore. They run here with Advanced settings, LoRAs, image to image and masked edits. Like LoRAs, they come straight from Civitai (not through Tor), and each is about 2 to 7 GB.
- **Bring your settings:** import a picture or workflow from A1111, Forge, Civitai or ComfyUI, or use a Civitai picture's settings in one click. Anything that can't come over (a ControlNet, say) is named.
- **Search Hugging Face** from the Models sheet: each image model shows its size and whether it runs on this PC.
- **Connect an agent:** Claude Desktop, Cursor or OpenCode can make pictures with the models on this PC, free. Connect gives you the setup to paste.
- **A quicker chat bar:** with nothing selected, the shortcut no longer stops to copy first, and the bar opens in front of your apps.
- **Cloud models with logos:** the model picker shows each cloud model's provider logo and name, without the route or context size.
- **Fixes:** Imagine's Advanced settings show their controls again, Reuse settings brings back the prompt and model, and Civitai searches filter and page correctly.

## New in 1.1.18

- **Imagine: pictures made on this PC** with image models you install. Upscale x2 or x4, vary or expand a picture in one click, start from a template, or sketch with **Draw** (it needs an edit model).
- **Explore:** find LoRA add-ons on Civitai and Hugging Face. Only .safetensors files install, each checked against its SHA-256. Civitai is reached straight from this PC, not through Tor, so Civitai sees your IP address and what you search. Mature pictures stay hidden until you turn on the 18+ setting.
- **A browser pane beside the chat:** watch the private browser live, open up to four tabs, and take control when you want. Password fields, and fields the site marks as one-time codes or card details, are hidden in the live view and masked from what the AI reads back.
- **Locked folders:** a locked folder's chats open only with your lock password, on this PC and on a paired phone. Chats from the chat bar now go into their own **Bar** folder.
- **Settings in your pictures:** saved pictures keep their settings and prompt in the PNG file. It's on by default; turn off **Embed settings in saved images** to stop it.
- **Connector permissions:** each connector has its own tool permissions, and you can ask again for a tool you allowed.
- **Older chats:** the sidebar shows your 200 newest chats and every chat in a folder or pinned; **Show older chats** brings in the rest. A message you are reading stays put when a reply finishes.
- **Calmer wording:** shorter, clearer text across the app, Eject without a popup, and the model picker centred.

## New in 1.1.17

- **Smarter computer use:** the assistant now uses an exact calculator for totals with tax or delivery, price comparisons and free calendar times, and it touches nothing on screen, so it asks for no approval card. In our tests with the 27B model, pass rates were the same or better and tasks took about 11% less time on average.

## New in 1.1.16

- **A more capable chat bar:** click the flamingo for a new chat; **Tools** lets a bar chat use web research or computer use (approvals still apply); **+** in the model list offers the model browser or an API provider.
- **Exclusive mode, redesigned:** one compact row per app, with its own icon and its share of graphics memory.
- **Models in one row:** Recommended, All, Installed, Filters and Sort on one line; capability filters moved into Filters.
- **Connectors with real logos:** two columns of cards, each with its service's own logo (Gmail, Outlook, Microsoft 365, Google and more), all built into the app.
- **A quicker start:** Foldmate opens sooner after a double-click (in our tests, the model's name shows about half a second sooner).
- **Fixes:** the chat bar's shortcut works over the desktop and maximized apps; memory checks before loading now default to **Relaxed**; a shorter note in temporary chats.

## New in 1.1.15

- **Mac preview updated to 1.1.15:** `Foldmate-1.1.15-mac.dmg` is on the [1.1.15 release](https://github.com/griffin300/foldmate-releases/releases/tag/v1.1.15). Computer use, Share control and the screen-saver handling for your phone are Windows-only, so the Mac version doesn't show them.
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

1. Open the **latest release** on this page and download `Foldmate-Setup-1.1.35.exe` under **Assets**.
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
| Imagine models and Explore (Hugging Face) | You download a model or browse Explore | The same route as models |
| Explore (Civitai) | You browse or install from Civitai | Direct only (Civitai sees your IP address and what you search). With Through Tor on, Civitai isn't used |
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

From 0.4.0 on, most updates download only the files that changed. 1.1.35 isn't one of those: every version
downloads the full installer (about 0.89 GB) to update.

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

## The tray, the chat bar and Quick actions

- **The tray:** right-click Foldmate's icon by the clock for **Open Foldmate**, **Load model**, **Chat bar**,
  **Eject model**, **App settings** and **Quit Foldmate**. Quit unloads the model and stops web research, so
  their memory is free again.
- **The chat bar:** press **Alt+\`** (the key under Esc). Alt+Space, Ctrl+Alt+F and Ctrl+Alt+B are choices in
  **App settings › This computer**. Text you highlight while it's open joins your question.
- **Quick actions:** select text in any app and press **Ctrl+Alt+Space** to proofread, rewrite, summarize, explain or
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
