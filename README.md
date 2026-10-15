# LeastCount

Coding up the most basic card game so my non-co-located friends can shit on each other.

That line is the whole original README. Pranav Prem committed it on January 23, 2022, along with GitHub's Python `.gitignore` template, and the repository has not grown since. This refresh documents that stub. It does not add the game.

## What it is

Least Count is a multiplayer card game played widely in India and among the diaspora. Everyone is dealt a hand from a standard deck, then draws and discards, trying to finish with the lowest point total. A player who thinks they are lowest can declare ("show"). Declare too early, or tie someone who is already lower, and the penalty is yours. Match play is usually a race in the other direction: accumulate too many points across hands and you are out.

House rules are the game. Hand size, how many decks, whether jokers are wild, whether you may drop several cards of the same rank, what an ace or a face card is worth, the cutoff for a legal show, and the penalty for a bad one all change from table to table. None of that was written down in this repo. The name and the one-line pitch are the only design notes on record: a shared table for friends who were not in the same room.

## How it works

It does not, yet. There is no rules engine, no deck, no scoring, no networking, and no interface. Nothing in git history was removed; the initial commit is still the only one that introduced files, and those files were the README and `.gitignore`.

## How to run it today

There is nothing to install, build, or start. Cloning the repository is the whole setup:

```bash
git clone https://github.com/pranavprem/LeastCount.git
cd LeastCount
```

You will have this documentation and a Python ignore file. No interpreter version is pinned, because no program was ever added.

## Tech stack

No language, framework, or dependency was committed. The Python `.gitignore` is the stock template GitHub offered for a new Python repo in 2022, refreshed here to the current template. It records the language that form suggested.

## Project structure

```
.
├── .gitignore   # current GitHub Python template, plus a few local extras
├── AGENTS.md    # guide for AI agents working in this repo
├── CLAUDE.md    # pointer to AGENTS.md
└── README.md
```

There is no UI, so there are no screenshots.

## Status

Still an idea. Implementing Least Count means choosing one rules variant first, then adding code. This repository does not do either.
