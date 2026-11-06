# Dustin Ingersoll

I build small AI systems end to end — engine, benchmark, tests, deployment — and publish the
numbers, including the experiments that lost.

## Projects

**[five-hundred-ai](https://github.com/dustin5551212/five-hundred-ai)** — 45-card 500, in Python

Three agents measured against each other on the same paired deals. Monte Carlo search beats the
hand-tuned CPU by **+0.98 tricks per deal** (95% CI 0.83–1.13) at 24 worlds; a behaviour-cloned
policy trained on that same CPU scores **−0.58**. 119 tests, seeded and reproducible.
[Play it](http://malls-mpegs.tun.ply.gg:28879/?ai=1) — every move there is the search agent's.

**[kings-corner](https://github.com/dustin5551212/kings-corner)** — Bicycle's rules, two to four players

Python server and a browser table, 39 tests. [Live table](http://jensen-shifted.tun.ply.gg:7251).

**Golf** — six-card Golf, nine holes

JavaScript reference implementation, plus a Python port kept honest by a parity fixture that
generates its expectations from the JS source. 53 tests.
[Live table](http://domination-grind.tun.ply.gg:53177).

## How I work

Benchmarks pair deals and share random numbers across candidates, because several of the bugs I
found were in the measuring rather than the model. Negative results stay in the repo with a
diagnosis instead of being deleted.

The tables above run from a desktop, so they are up only while it is — the code and the tests are
the durable part.
