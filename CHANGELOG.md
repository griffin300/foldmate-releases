# Foldmate changelog

What changed in each earlier version of Foldmate, newest first. The latest version's notes are in the [README](README.md).

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
