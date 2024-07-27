# The Sacred Timeline (an MCU git history)

A joke repo that models the Marvel Cinematic Universe's continuity as an
actual git history — branches for Nexus Events, merges for the multiverse
reconverging, tags for each Phase, and real content files (not just empty
commits) so `git log -p`, `git show`, and `git diff` all tell part of the story.

## Explore it

```bash
git log --all --graph --oneline --decorate
git tag -l
git checkout earth-838
git diff phase-3 phase-4 -- characters/
```

## Structure

- `movies/phaseN/*.md` — one file per film: cast, director, box office, synopsis
- `characters/*.md` — bios, added at first appearance, removed/restored around the Snap
- `events/*.md` — Nexus Event write-ups on the branch commits
- `posters/` — drop your own official poster images here (see posters/README.md)

## Branches

| Branch | What it represents |
|---|---|
| `main` | The Sacred Timeline (primary MCU continuity) |
| `thanos-2014-heist` | The 2014 Thanos variant's alternate branch, pruned after Endgame |
| `loki-tva-timeline` | The 2012 Loki variant's escape, the seed of the TVA storyline |
| `earth-838` | The alternate universe visited in Doctor Strange 2 |

## Tags

`phase-1` through `phase-5`, each pointing at that Phase's closing film.
