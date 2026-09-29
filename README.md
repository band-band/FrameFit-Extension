# FrameFit Extension

Current version: **2.4.2**

[Download FrameFit Extension.zip](./FrameFit%20Extension.zip?raw=true)

FrameFit lets you watch video in a compact browser window, fill the current tab, or use native Picture-in-Picture. Includes global and per-site switches and four menu themes.

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

Version 2.4.2 removes the floating Minimize control and fully removes the compact tip panel when dismissed. This distribution contains the unchanged 2.4.2 extension.

[Privacy policy](PRIVACY.md)
