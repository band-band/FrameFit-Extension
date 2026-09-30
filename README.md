<img src="./framefit-logo.png" alt="FrameFit logo" width="80" height="80">

# FrameFit Extension

Current preview: **2.6.0**

[Download FrameFit Extension.zip](https://github.com/band-band/FrameFit-Extension/releases/download/v2.6.0/FrameFit.Extension.zip)

Use this direct download to install FrameFit. GitHub's **Code > Download ZIP** and
**Source code (zip)** download the repository, which contains the extension ZIP.
The direct download contains `manifest.json` and the extension files, with no ZIP inside.

Make room to watch. FrameFit turns supported video fullscreen buttons into
**Theater Mode**, **Tab View**, or native **Picture in Picture**.

## Studio menu

<img src="./framefit-studio-dark.png" alt="Studio Dark menu in charcoal and lavender" width="352">
<img src="./framefit-studio-light.png" alt="Studio Light menu in white and blue" width="352">

The new menu has a visual mode preview, a larger green master switch, and settings
behind the gear. Choose **Studio Dark** or **Studio Light**. Fonts are bundled
locally. **Takeover** now offers an always-on-top player with custom controls.

## Takeover

Takeover opens an always-on-top Document Picture-in-Picture window with FrameFit's
play/pause, seek, mute, volume, and Return to tab controls. Select Takeover, enable
the site, then use the video's fullscreen button or Alt+Shift+V. The existing
native Picture in Picture mode remains available separately.

Esc, Return to tab, or closing the floating window restores the original video.
Navigation closes Takeover so the site can load its next page normally. Chrome
controls the floating window's position and size limits; it does not follow the
browser. It requires Document PiP support and a top-level video page. Embedded or
restricted videos may not work. Site quality menus, playlist controls, and captions
drawn outside the video are not copied. Seeking is disabled for indefinite live streams.

## Install

1. Download **FrameFit Extension.zip** above and extract it into a permanent folder named **FrameFit Extension**.
2. Open `chrome://extensions` in Chrome and enable **Developer mode**.
3. Click **Load unpacked** and select the extracted folder containing `manifest.json`.
4. Refresh existing video tabs and pin FrameFit from Chrome's Extensions menu.
5. Open FrameFit on a video website and turn on **Enable on this site**.

Keep the extracted folder in place. Chrome loads the extension from that folder.
Requires Chrome 119 or later. Websites start off until you enable them.

## Use and update

Choose a viewing mode, then click a video's fullscreen button or use **Alt+Shift+V**.
Theater Mode fills the page while keeping browser controls. Tab View puts the
same video tab in a separate window with Chrome's title and URL bars. Picture in
Picture floats above other apps; some videos do not allow it.

In Tab View, **Return to tab** or **Esc** restores the page and returns the same
video tab. The window's native **X** closes the video tab. Close confirmation
defaults on, but Chrome controls when its generic Leave/Cancel warning appears.
Settings includes close confirmation and a switch to restore hidden Tab View tips.

For updates, exit Tab View, replace the contents of your existing installation
folder with the new package, reload FrameFit at `chrome://extensions`, and refresh
video tabs. **After upgrading to 2.5.0, enable each video website in the menu.**
Global, viewing-mode, close-confirmation, and tip preferences are retained.
The old Chrome light palette becomes Studio Light; other old palettes become
Studio Dark.

## About this download

This repository distributes the installable extension only. Development tools,
tests, editable artwork, and development history are maintained separately.
The ZIP necessarily includes the JavaScript, HTML, CSS, fonts, and images Chrome
runs; those bundled files can be inspected.

Version 2.5.2 repairs stale YouTube player sizing when switching to the next video.
53 YouTube fixture checks passed, including next-video transitions in both modes.
Real YouTube transitions still need an installed-extension smoke test.

Version 2.5.1 corrects the mode names without changing your saved selection or player behavior.

Version 2.5.0 redesigns the menu and adds explicit site opt-in. It retains the
YouTube sizing and X playback repairs from 2.4.6. Takeover is added in 2.6.0.
The floating Minimize control remains removed.

35 background/settings tests, 20 dedicated Takeover fixture checks, and the 23-file package audit passed. Real Document PiP opened a generated video and restored it in the in-app browser. Takeover is a preview pending real-site compatibility checks. Generic player and Twitch regression runs were inconclusive due to loaded-extension interference; see the release notes. The implemented popup
was checked in a browser fixture with simulated Chrome APIs, including both
themes, preference saving, site opt-in, unsupported pages, and loading/saving
errors. This is not installed-Chrome verification; the native popup and close
dialog still need a real Chrome smoke test. Earlier player checks were not rerun
for this menu update.

[Privacy policy](PRIVACY.md)
