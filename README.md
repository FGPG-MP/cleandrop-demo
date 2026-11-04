# Clean Drop — demo

Password-protected builds; everything under `c/` is encrypted and each password is shared separately from its link.

- `/` — the game wall (present mode)
- `/dashboard/` — the event dashboard, review copy (nothing is sent to any station)
- `/trivia/` — the trivia kiosk, review mode (`trivia.html?demo`: no station; R shows the review bar). The film here is a web encode of Chevron's, unedited, to stay under GitHub's 100 MB file limit.

- `/next/`, `/next/trivia/` — review builds, for FGPG's yes before they reach Chevron

Rebuilding the game at the root: rsync with `--exclude .git --exclude README.md --exclude dashboard --exclude trivia --exclude next`, or `--delete` wipes the others.

Built 3 Nov 2026 from the game repo `main` @ 3bef6a9 (Chevron's 2 Nov notes): the game in whack mode, the trivia kiosk with the web encode of the film. The root and `/trivia/` are byte-identical copies of `/next/` and `/next/trivia/`, moved up on Nick's word. `/dashboard/` is still the 16 Oct build (`main` @ a8a79cd).

