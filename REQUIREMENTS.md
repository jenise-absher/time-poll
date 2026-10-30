# Find-a-Time: requirements

A small, free site that helps a few friends find a time to meet.
A learning project for GitHub and Netlify. No accounts, no emails, no cost.

## How it works

1. **Start.** The first screen asks: create a new poll, or enter the code for one you already made.
2. **Create.** Give it a title, pick a few days and the hours to choose from.
3. **Save your code.** You get a short private code (like `K7M-Q2X`). You need it to come back. You can't move on until you copy it or tick "I've saved it."
4. **Share.** Then you get a link for your friends (up to 5). Send it however you like.
5. **Answer.** Friends open the link, type a name, and tap the times they're free.
6. **Pick.** Enter your code on the start screen to see the results and choose a time. Download a calendar file to share.

Polls are deleted after 30 days.

## Keeping the code and the link apart

The code is yours. The link is for friends. They should never be mixed up.

| | Your code | Share link |
|---|---|---|
| Who it's for | Only you | Your friends |
| Icon | Key | Paper plane |
| Look | Gold, striped, dashed edge, like a ticket | Plain white card |
| When | Step 1, on its own | Step 2, after the code is saved |

## Look and feel

- Calm and plain: no colored header bars, lots of white space.
- Works on a phone.
- Show times in each person's own time zone.

## Not doing

Logins, sending emails or texts, reminders, calendar sync, anything private in the title.

## Build steps

1. ~~Hello page on GitHub.~~
2. Connect to Netlify.
3. Start screen and create-poll page.
4. Save polls with a Netlify Function and Blobs. Return the code and the link.
5. Answer page.
6. Results and pick a time.
7. 5-person limit and 30-day cleanup.
