# Clean Drop — demo

Password-protected builds; everything under `c/` is encrypted and each password is shared separately from its link.

- `/` — the game wall (present mode)
- `/dashboard/` — the event dashboard, review copy (nothing is sent to any station)
- `/trivia/` — the trivia kiosk, review mode (`trivia.html?demo`: no station; R shows the review bar). The film here is a web encode of Chevron's, unedited, to stay under GitHub's 100 MB file limit.

Rebuilding the game at the root: rsync with `--exclude .git --exclude README.md --exclude dashboard --exclude trivia`, or `--delete` wipes the other two.

Built 16 Oct 2026 from the game repo `main` @ a8a79cd (the final logos, the NEXT-GEN lockup on the trivia kiosk, the logo on the sign-in page): the game in whack mode, the trivia kiosk with the web encode of the film, and the dashboard review copy. `brand.png` is the sign-in page's logo and ships unencrypted.

