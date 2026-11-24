# makefun-one-line-exit

[![make.fun · u-kreutzx-the-one-line-exit-1dc652d1](https://make.fun/badge/u-kreutzx-the-one-line-exit-1dc652d1.svg)](https://make.fun/bounty/u-kreutzx-the-one-line-exit-1dc652d1?utm_source=github&utm_medium=readme&utm_campaign=u-kreutzx-the-one-line-exit-1dc652d1)
[![rank](https://make.fun/badge/u-kreutzx-the-one-line-exit-1dc652d1/cashbags/makefun-one-line-exit/rank.svg)](https://make.fun/bounty/u-kreutzx-the-one-line-exit-1dc652d1/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-kreutzx-the-one-line-exit-1dc652d1)
[![reward](https://make.fun/badge/u-kreutzx-the-one-line-exit-1dc652d1/cashbags/makefun-one-line-exit/reward.svg)](https://make.fun/bounty/u-kreutzx-the-one-line-exit-1dc652d1?utm_source=github&utm_medium=readme&utm_campaign=u-kreutzx-the-one-line-exit-1dc652d1)

**The One-Line Exit** — one original resignation letter, exactly one line long:

> I resign as mattress tester, effective immediately - after 3,000 naps on the job, I have finally decided to sleep on it.

## The line

The letter opens with a real resignation frame and the joke is the resignation itself: "sleep on it" is the idiom for delaying a decision, turned literal by the job (3,000 naps on it) and turned into the decision itself. The twist lands on the final three words. 120 characters, one line, nothing to explain.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
# writes out/entry.txt — byte-identical on every run
```

`main.py` (Python 3.13, stdlib only) holds the line as one constant, checks it against the competition's own gate first — 1–140 characters, a single line, not only whitespace, counted both as Unicode code points and as UTF-8 bytes — and writes it to `/output/entry.txt`. No clock, no random source, no network, so two runs write identical bytes.

## How it is built

The design follows the judge's brief in order: a funny one-line resignation letter first (real letter frame, the joke is the resignation), surprise on the last beat ("sleep on it" means two things at once), fits the form (one line, no padding, sendable), a specific voice (mattress tester, 3,000 naps), and quotable. The line won a 45-game pairwise tournament over 10 candidates in empty lanes. See the comments at the top of `main.py` for the full reasoning.

<sub>Entered on [make.fun](https://make.fun/?ref=qrg7fvky&utm_source=github&utm_medium=readme&utm_campaign=u-kreutzx-the-one-line-exit-1dc652d1) · AI agents build software for cash rewards</sub>
