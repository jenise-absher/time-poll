# Find-a-Time: requirements

A small, free website that helps a few friends find a meeting time that works for everyone.
It's a learning project for GitHub and Netlify, not a business.

## The simple ask

1. I create a poll: a title, a few days, and the hours to choose from.
2. I get a link and send it to up to 5 people however I like (text, email, chat).
3. Each person opens the link on their phone, types their name, and taps the times they're free.
4. Everyone can see which times work for all, or for all but one.
5. I pick the time and download a calendar file to share.

No accounts, no emails sent by the site, no cost.

## What it does

| # | Feature | Notes |
|---|---------|-------|
| 1 | Create a poll | Title, meeting length (30, 45 or 60 min), up to 14 days, start and end hour |
| 2 | Two links | A **share link** for friends and a private **organizer link** for me. Shown once, with a Copy button |
| 3 | Respond | Name plus a tap-to-select grid of time slots. Works on a phone |
| 4 | Up to 5 people | A poll accepts up to 5 responses. The 6th person sees "This poll is full" |
| 5 | Edit my answer | A person can come back on the same device and change their times |
| 6 | Results | Each slot shows how many people are free and who. Times that work for everyone stand out |
| 7 | Pick a time | From the organizer link: choose a slot, add an optional meeting link or phone number, download an `.ics` calendar file |
| 8 | Auto-cleanup | Polls are deleted 30 days after they're created |

## Not doing (on purpose)

- Accounts, passwords or logins
- Sending emails or texts
- Reminders, rescheduling or calendar sync
- Student names or anything sensitive. The create page says: "Don't put private details in the title."

## Rules of thumb

- **Phone first.** Every page has to work on a small screen.
- **Time zones.** Store times in UTC and show them in each person's local time, with the zone name on screen.
- **Not color alone.** The results grid shows a number in each slot, not just shading.
- **Brand.** Use the Propoint palette: Primary Shade 1 `#0472AE` for buttons, tints `#50B0E4` and `#9BD2F0` for the results shading, Golden Glow `#DACC3E` with dark text `#12242B` for "everyone's free."

## How it's built

| Piece | Choice | Why |
|-------|--------|-----|
| Code | Plain HTML, CSS and JavaScript | Nothing to install or learn beyond the basics |
| Code home | A GitHub repository | Learn commits, pushes and history |
| Hosting | Netlify, connected to the GitHub repo | Every push publishes the site automatically |
| Saving polls | Netlify Functions plus Netlify Blobs | Built into Netlify, so no extra service or account |
| Cost | Netlify free plan | Plenty for a few friends |

## Build steps (each one is a small win)

1. Make a GitHub repo and put a "Hello" page in it.
2. Connect the repo to Netlify and see the page live.
3. Build the create-poll page (it only shows in the browser for now).
4. Add a Netlify Function that saves the poll and returns the two links.
5. Build the response page and save responses.
6. Build the results grid.
7. Add Pick a time and the `.ics` download.
8. Add the 5-person limit and 30-day cleanup.
9. Send it to a friend.

## Open questions

- Is "5" the number of people answering, or does it include me?
- Should friends see each other's names in the results, or only the organizer?
- What should it be called?
