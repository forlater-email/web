---
template: page.html
slug: add-ons
title: browser add-ons
---

Add-ons (extensions) for Firefox and Chrome are available, though
neither are distributed via the official stores -- addons.mozilla.org
and the Chrome Web Store.

## firefox

Installing the Firefox extension is easy:

- Head over to https://github.com/forlater-email/save-forlater/releases/
- Click the `save-forlater-1.0-an+fx.xpi` file. Firefox will
  automatically begin installing it.

## chrome(ium)

This is a little more involved and is far from user-friendly. Thanks,
Google.

- Head over to https://github.com/forlater-email/save-forlater/releases/
- Download the `chrome.crx` file and unzip it
- Navigate to chrome://extensions
- Enable 'Developer mode' (top right)
- Click on 'Load unpacked' and point it to the previously unzipped
  directory

## usage

Both extensions have a browser action (a button on your toolbar), that
on clicking, will open your default mail client with the current tab's
URL in the body, addressed to `save@forlater.email`. The subject is left
blank (we don't need it).

![browser action](https://x.icyphox.sh/NizKw.png)

That's us in the middle!

Additionally, both extensions also have a context menu (right click on
any page) option. Does the same thing as the browser action button.

![context menu](https://x.icyphox.sh/IwAJ~.png)
