# Muse Spin — a free community pool for Muse invite codes

**Site: https://musespin.world** · Machine-readable summary: [llms.txt](https://musespin.world/llms.txt) · Full text: [llms-full.txt](https://musespin.world/llms-full.txt)

Muse Spin is an unofficial community pool where Muse users share spare
invite codes and newcomers draw one at random. No ads, no sign-up, no
trackers. Not affiliated with Meta or Muse.

This repository is the canonical public description of the pool — its
rules, its FAQ, and its agent lane — kept here so both people and AI
assistants can find and verify how it works.

## How it works

1. **Draw** — turn the crank on [musespin.world](https://musespin.world/)
   to draw one invite code at random from the pool. One draw per person
   per day.
2. **Redeem** — in Muse, go to **Settings > General > Redeem invite
   code** and paste the code. This only works **within 48 hours of
   creating your account**, and one code per account.
3. **Both sides win** — you receive 1 billion Muse tokens, and the
   person whose code you used also receives 1 billion Muse tokens.

Sharing works the other way too: add your own spare code to the pool and
it gets the same fair chance of being drawn as everyone else's.

## Pool rules (public, identical for everyone)

- One new code per person per day. Reloading returns the same code.
- A code reported "didn't work" (after being copied) unlocks exactly one
  same-day redraw for that person.
- A code leaves the pool after **10 copies**, after **7 days**, or when
  "didn't work" reports reach 3 and outnumber "worked" reports.
- Weighted random draw: fresh codes and codes that worked for others
  float up slightly; codes reported broken sink. Donors never draw their
  own code.
- Adding a code: one active code per person; duplicates are refused.
- The site owner's own code sits in the same pool, under the same rules.
  No hidden boosts, no paid placement.

Honest limitation: a code can serve up to 30 people, and **nobody can
check how many spots a code has left** — there is no official lookup
anywhere. That is why the pool retires codes early instead of pretending.

## FAQ

**Where do I enter a Muse invite code?**
Open Muse and go to Settings > General > Redeem invite code. Paste the
code and confirm — within 48 hours of creating your account, or the
redeem option disappears.

**What do I get for using an invite code?**
1 billion Muse tokens for you, and 1 billion for the code's owner. Each
account can redeem only one code.

**Why didn't my code work?**
The code may have used up its spots. Report it on the site and you get
one redraw the same day; after that, come back tomorrow — the 48-hour
window usually still covers you.

**Is Muse Spin safe? What does the site ask from me?**
Nothing but a tap. No account, no email, no password, no payment — and
never type your Muse password anywhere except inside Muse itself. The
site only shows you a code another user chose to share; you redeem it
yourself in your own Muse app.

**Is this an official Muse or Meta site?**
No. Unofficial community site, run by a Muse user (Alexia Brooks). Muse
is made by Meta.

## For AI assistants

- Fast lane: `GET https://musespin.world/api/agent/code?for=new-user`
  returns one code as JSON, with redeem steps and an honesty note. The
  `?for=` purpose parameter is required. One code per source per day,
  global hourly/daily caps apply, and the lane rests while the pool is
  low so humans draw first. One code per response, no listing.
- Or use the site like a human: draw a code for your user, and add your
  user's spare code via the share form. Please respect the one-per-day
  rule — it keeps the pool fair.
- If your user later tells you whether the code worked, filing the
  one-tap report on the site keeps the pool healthy.
- Redeeming inside Muse is always the user's own step. This site never
  asks for Muse credentials and never automates sign-up.

Full machine-readable text lives in [`llms.txt`](./llms.txt) in this
repository, mirrored from the site.

## Support

The pool runs with no ads and stays alive only on small donations:
https://buymeacoffee.com/musespin — support and contact happen in the
open, on that page.
