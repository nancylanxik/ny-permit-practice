# NY Permit Practice Quiz 🚗

A free, open-source practice quiz for the **New York State driver's permit (written knowledge) test**. It runs entirely in your browser — no install, no account, no internet required after loading. Your progress is saved locally.

👉 **[Try it live](https://nancylanxik.github.io/ny-permit-practice/) 

![one-page cheat sheet](cheatsheet.pdf)

## Features

- **250+ practice questions** across every topic on the NY permit test (traffic control, intersections & turns, passing, parking, defensive driving, alcohol & drugs, special conditions, sharing the road, road signs, plus NYC-specific rules).
- **Hand-drawn road-sign questions** (SVG) so you learn to recognize signs by sight.
- **Five study modes:** Quick 10, Full 20 (exam simulator), Full Coverage, **Endless Practice** (serves unseen questions first), and **Review My Mistakes**.
- **Mastery tracker** — a progress bar and per-topic coverage chart show exactly what you've learned. Saved in your browser (localStorage), so it persists between sessions.
- **Mistake Bank** — every question you miss is saved automatically for targeted review.
- **Instant feedback** with a short explanation for every answer.
- **One-page printable cheat sheet** (`cheatsheet.html` / `cheatsheet.pdf`).

## How to use

**Option 1 — just open it:** download the repo and double-click `index.html`. It opens in any browser.

**Option 2 — host it free with GitHub Pages:**
1. Push this repo to GitHub.
2. Go to **Settings → Pages**, set the source to your `main` branch (root).
3. Your quiz will be live at `https://<your-username>.github.io/<repo-name>/`.

## Contributing

Questions, fixes, and new items are welcome! Each question lives in the `BANK` array inside `index.html` in this format:

```js
{ id:"q42", t:"Ch 4: Traffic Control",
  q:"A flashing red traffic light means:",
  opts:["Slow down","Stop, then go when safe","Ignore it","Speed up"],
  a:1,                                  // index of the correct option
  e:"A flashing red light works exactly like a STOP sign." }
```

Add `sign:1` and an inline `svg:"<svg>...</svg>"` for picture-based road-sign questions. Open a pull request with your changes.

## Sources & disclaimer

- Questions and rules are based on the **official [New York State Driver's Manual (MV-21)](https://dmv.ny.gov/new-york-state-drivers-manual-practice-tests)** and the NY DMV chapter practice quizzes. Facts were verified against the manual.
- This is an **unofficial study aid**. It is **not affiliated with, endorsed by, or connected to** the New York State DMV or any government agency.
- The real test draws its own questions from the DMV's pool — these are practice questions to help you learn the rules, not the actual exam items.
- Provided **as-is, with no warranty**. Always confirm current rules, fees, and procedures at [dmv.ny.gov](https://dmv.ny.gov).

## License

Code is released under the **MIT License** — see [LICENSE](LICENSE). You're free to use, modify, and share it. A credit link back is appreciated but not required.

---

*Built as a personal study tool and shared so others can pass their permit test too. Good luck! 🍀*
