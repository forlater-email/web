---
template: page.html
title: forlater.email
subtitle: email-based bookmarking service
---

## what?

forlater is an email-based bookmarking service. You send us an
email with a link (or links), and receive a readable, clutter-free
version of the article in an email.

This is a *"paid service"* -- you just pay how much ever you want via
[Liberapay](https://liberapay.com/icyphox/donate). I insist that you try
it out before you pay; you can better gauge how much value you derive
from forlater. It's completely fine if you don't want to pay too!

## how does it work?

Easy. Do this:

- Grab a link. Copy it to your clipboard, use your phone's share-menu,
  whatever.
- Compose an email using any mail client to `save@forlater.email` with
  the link in the body. The subject doesn't matter.
- Hit send and give it a moment.

All emails are both `text/html` and `text/plain`. The plaintext is
optimized for maximum readability, with all images and links converted
to footnotes. The HTML is minimally styled, and should look fine in just
about any mail client.

## but why email?

The reason is simple: you get organization for free. All mail sent by us
originate from `saved@forlater.email` (notice `saved`!), and you can
filter these however you like.

For example, here's a [sieve](http://sieve.info/) filter for redirecting
mail from `saved@forlater.email` to a folder called `Read Later`.

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

## important notes

forlater is still beta quality software. The web is hard, and so is
email. Some pages might not get parsed properly; if you're trying to
save pages that don't primarily have much text, it probably won't work
very well.

## FAQs

They're not really that frequent.

### how is this better than Pocket?

Let's see...

- You own your data. It lives right in your inbox!
- You don't need yet another account or app. Just simple email.
- We're open source!

That said, Pocket has a full-fledged engineering team working on it, so
their article parsing is probably better.

### are you tracking me?!

Nope. You can audit our code [here](https://github.com/forlater-email).
However, for the moment, we're using [Mailjet](https://mailjet.com) for
outbound email. All tracking is turned off, and we only use the SMTP
relay.

I'd really like to move away from them and host my own server, in
the near future.

### are you open source?

Yes, as mentioned previously (twice!), we are open source -- licensed
under (A)GPL. See:

- https://github.com/forlater-email
- https://git.icyphox.sh/forlater

### you keep saying 'we'; how many of you are there?!

I'm just [one guy](https://icyphox.sh). 'We' just sounded right, I
guess.  Feel free to email me at [x@icyphox.sh](mailto:x@icyphox.sh) to
report any issues.
