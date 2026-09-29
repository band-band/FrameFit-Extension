<img src="./framefit-logo.png" alt="FrameFit logo" width="80" height="80">

# FrameFit Extension

Current version: **2.4.6**

[Download FrameFit Extension.zip](./FrameFit%20Extension.zip?raw=true)

FrameFit lets you watch video in a compact browser window, fill the current tab, or use native Picture-in-Picture. Includes global and per-site switches and four menu themes.

## Menu preview

<img src="./framefit-menu.jpg" alt="FrameFit menu in Light purple, showing viewing modes and per-site settings" width="360">

## Install

1. Download **FrameFit Extension.zip** above and extract it into a permanent folder named **FrameFit Extension**.
2. Open `chrome://extensions` in Chrome and enable **Developer mode**.
3. Click **Load unpacked** and select the extracted folder containing `manifest.json`.
4. Refresh existing video tabs and pin FrameFit from Chrome's Extensions menu.

Keep the extracted folder in place. Chrome loads the extension from that folder. Requires Chrome 119 or later.

## Use and update

Click a video's fullscreen button, or use **Alt+Shift+V**. Select your preferred viewing mode in FrameFit's menu.

In compact view, **Return to tab** or **Esc** restores the page and returns the same video tab. The window's native **X** closes the video tab. Close confirmation defaults on, but Chrome controls when its generic Leave/Cancel warning appears.

For updates, exit compact view, replace the contents of your existing installation folder with the new package, reload FrameFit at `chrome://extensions`, and refresh video tabs. Keeping the same installation folder helps retain preferences.

## About this download

This repository distributes the installable extension only. Development tools, tests, editable artwork, and development history are maintained separately. The ZIP necessarily includes the JavaScript, HTML, CSS, and images Chrome runs; those bundled files can be inspected.

Version 2.4.6 fixes X black screens caused by page updates and preserves already-playing videos during expansion, while respecting manual pause. It retains explicit YouTube video and control sizing on entry and after Escape or fullscreen-button exit, including later browser resizing in both Fill current tab and compact mode. It retains the previous improvements: FrameFit opens compact view in a smaller normal window, handles responsive YouTube player moves, keeps its bottom controls inside the player, and makes its fullscreen button toggle back out. X/Twitter uses its video-and-controls component for expansion and supports the English-labeled fullscreen toggle. The floating Minimize control remains removed.

Targeted X class-replacement and playback-recovery fixtures passed, and live X playback continued through repeated expansion and exit without a manual Play click in the in-app browser. The full X fixture remains inconclusive because the installed extension interferes with its keyboard check. Native compact-window playback and Chrome dialogs still need separate verification. Previous YouTube validation is recorded in the development repository.

[Privacy policy](PRIVACY.md)
