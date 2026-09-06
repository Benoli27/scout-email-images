# Scout email images

Pictures used in emails sent from the
[Scout Email Generator](https://github.com/Benoli27/Scout-Email-Generator).

This repository is public and contains **only images**, so nothing else has to
be. Emails fetch their pictures when the recipient opens the message — sometimes
months after it was sent — so the addresses here need to keep working long after
the email has gone.

## What must never go in here

**No photographs of young people.** Anyone with the address can view these
files, and search engines can index them. Group logos, campsite pictures, badge
artwork and scenery are fine. Photographs of Scouts are not, whatever the photo
permissions say — a public folder is the wrong place for them.

Nothing with personal details either: no scans of forms, registers, consent
slips or medical information.

## Adding a picture

1. Put the file in the folder that fits: `logos/`, `banners/`, `badges/` or
   `photos/`.
2. Name it in lowercase with hyphens and no spaces — `summer-camp-2026.jpg`,
   not `Summer Camp 2026 (final).JPG`. Spaces and capitals cause trouble in web
   addresses.
3. Commit and push.
4. In the generator, type the short path with a leading slash:

   ```
   /banners/summer-camp-2026.jpg
   ```

   The field will show you the full address it will actually be sent as.

Allow a minute or two after pushing — GitHub takes a moment to publish.

## Checking it worked

**Open the address on your phone.** If the picture fills the screen, it will
work in every email client. If you get a web page, an error or a sign-in
prompt, it will show as a broken image for some of your recipients.

This is the test that matters. A OneDrive share link previously looked perfect
on a PC and in Gmail, and showed a broken image in Outlook and Safari on iPhone.

## Sizes

| Use | Width | Notes |
| --- | --- | --- |
| Banner | ~1200px | Displayed at 600px; the extra keeps it sharp on phones |
| Photos | ~1000px | Up to three sit side by side |
| Badges | ~300px | Displayed 80px tall |
| Logo | ~500px | Displayed 130px wide |

Keep each file under about 500KB. Large images make emails slow to open on a
phone, and some clients give up waiting.

## Deleting and replacing

Deleting a file, or renaming it, **breaks every email already sent that used
it** — those messages will show a broken image from then on. Add new files
rather than replacing old ones, and leave the old ones in place.

## Publishing setup

Done once, in this repository on github.com:

**Settings** → **Pages** → Source: *Deploy from a branch* → Branch: `main`,
folder **/ (root)** → **Save**.

Files are then served from:

```
https://benoli27.github.io/scout-email-images/
```
