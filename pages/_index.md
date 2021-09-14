---
template: page.html
title: forlater.email
subtitle: Email-based bookmarking service.
---

Email-based bookmarking service.

**NOTICE**: it's not up yet!

### save it for later

*TL;DR*: Send a link to `save@forlater.email` to get started!

Simply send an email with a link (or links; one per line) to
`save@forlater.email`, and you'll get a readable, clutter-free version
of it in your inbox. No tracking, no bullshit.

Don't like HTML email? Me neither, actually. I've got you covered: all
emails have both `text/html` and `text/plain` parts; plaintext content
is optimized for readability, with images and links as footnotes.

### organizing saved pages

All saved email come from `saved@forlater.email` (notice `saved`!). For
example, here's a [sieve](http://sieve.info/) filter for sending mail
from `saved@forlater.email` to a folder called `Read Later`.

```sieve
require ["fileinto", "mailbox"];
if address "From" "saved@forlater.email"
{
    fileinto :create "Read Later";
}
```

Or, if you use GMail, you can [create filter
rules](https://support.google.com/mail/answer/6579?hl=en#zippy=%2Ccreate-a-filter)
to automatically label mail from `saved@forlater.email`.

In short: do it however you like! That's the beauty of email.
