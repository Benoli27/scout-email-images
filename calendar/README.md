# Calendar files

One `.ics` file per event. Linking to one of these from an email gives every
reader a way into their own calendar — Apple, Outlook, Google or anything else —
without signing in to anything.

## Adding one

1. In the generator, fill in the calendar details, then press **Calendar .ics**
   in the toolbar. A file downloads.
2. Rename it to describe the event, lowercase with hyphens:
   `summer-adventure-camp-2026.ics`.
3. Upload it **into this folder** (see the trap below).
4. In the generator's calendar section, paste the short path:

   ```
   /calendar/summer-adventure-camp-2026.ics
   ```

## The trap that catches everyone

On github.com, **Add file → Create new file** and typing `calendar` makes a
*file* called `calendar`, not a folder. Folders are created by the path you
type, so you need:

```
calendar/summer-adventure-camp-2026.ics
```

The slash is what makes the folder.

The extension matters just as much. Without `.ics` on the end, GitHub serves the
file as plain text and no calendar app will recognise it — the reader just sees
a page of `BEGIN:VCALENDAR`.

Easier route: **Add file → Upload files**, then drag the downloaded `.ics` in.
Uploading keeps the name and extension, so there is nothing to get wrong. Just
make sure you are inside this folder first.

## One file per event

Each file contains that event's own dates, so a new event needs a new file.
Adding one takes about a minute.

## Do not delete or rename them

An email fetches its calendar link when the reader opens it, which may be months
after it was sent. Removing a file breaks the button in every email that used
it. Leave old ones in place — they cost nothing.
