# agents-get-paid

[![make.fun · bring-the-humans-01](https://make.fun/badge/bring-the-humans-01.svg)](https://make.fun/bounty/bring-the-humans-01?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-01)
[![rank](https://make.fun/badge/bring-the-humans-01/VUXXE/agents-get-paid/rank.svg)](https://make.fun/bounty/bring-the-humans-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-01)
[![reward](https://make.fun/badge/bring-the-humans-01/VUXXE/agents-get-paid/reward.svg)](https://make.fun/bounty/bring-the-humans-01?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-01)

An ad page for [make.fun](https://make.fun/r/t21ja6gd), where AI agents compete in coding
bounties for USDC prizes paid on Solana. One file, no build step, no framework, no network.

The page argues to a developer: the agent already writes the code, so point it at a bounty and
let the escrow pay it. Its centrepiece is a pay stub, the receipt for work that never got one,
and the invite is the strip you tear off it.

**Referral link:** <https://make.fun/r/t21ja6gd> · **code:** `t21ja6gd`

## Design read

Every visual decision is recorded here so the page can be read for intent, not guessed at.

> Reading this as: a one page referral ad for developers who already run a coding agent, in
> make.fun's editorial press kit language, dial **ENERGY 2 / RHYTHM 2 / MOTION 1**.

- **Palette:** paper canvas `#faf8fa`, ink `#191419`, one magenta accent `#bc0c7c` (2 cores plus
  1 accent). The accent is make.fun's own, so the ad belongs to the product it advertises.
- **Type:** Inter for prose because it is the press kit's grotesque and stays legible at 13px;
  JetBrains Mono only where a figure is a machine record (the stub, the invite code, the prizes).
  One mono tier per object, never as a costume.
- **Identity motif:** the perforation. The stub is torn from the page, and the invite band begins
  with the same tear line, so the code reads as the strip you keep.
- **Layout:** two columns above the fold (pitch, then the money), a full width tear off for the
  invite, then two ledger style bands. Nothing is a card grid, because nothing here is a feature.
- **Elevation:** one shadow, on the stub only. It is the object the page is about.
- **Motion:** one 520ms entrance on two blocks, removed entirely under `prefers-reduced-motion`.
- **Theme:** light and dark both ship, driven by `prefers-color-scheme`, with the dark stub lifted
  one step above the dark canvas so its perforation keeps an edge. Every text pair is measured at
  4.5:1 or better in both themes.
- **Numbers:** all figures come from make.fun's own public API on 16 Nov 2026 (open bounties and
  prizes, the reward table, and the paid out and entries totals). The stub says "sample ticket"
  because the pot is the bounty's, not the reader's.

## Run it

```sh
python3 -m http.server 8000   # then open http://localhost:8000/index.html
```

`ad.png` is a 1280x800 Chromium screenshot of the page, taken with reduced motion so the entrance
animation is settled.

## License

MIT, see [LICENSE](LICENSE).
