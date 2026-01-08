+++
title = "Contributions to Rust in 2025"
date = 2026-01-08
description = "Contributions to Rust in 2025"
+++

I saw other Rust maintainers posting their contributions in 2025, so I thought
why not join the party :)

# PRs authored

[261 PRs to various `rust-lang/`
repos](https://github.com/issues?q=author%3Ajieyouxu%20is%3Amerged%20merged%3A2025-01-01..2025-12-31%20org%3Arust-lang%20-label%3Arollup)

You can use queries like

```text
author:jieyouxu is:merged merged:2025-01-01..2025-12-31 org:rust-lang -label:rollup
```

on the <https://github.com/issues> page to look up your own contributions to
various repositories within 2025.

# PRs reviewed

[Approximately 680 `rust-lang/` PRs reviewed](https://github.com/issues?q=assignee%3Ajieyouxu%20is%3Amerged%20merged%3A2025-01-01..2025-12-31%20org%3Arust-lang)[^review-note]

```text
assignee:jieyouxu is:merged merged:2025-01-01..2025-12-31 org:rust-lang
```

# Summary

I do `$random_contributions` around the Rust project, based on `$vibes`[^vibes].
My style of contribution is probably most accurately described as "efforts
towards enabling other contributors", since I mostly work on the test
infrastructure (`compiletest` and friends), the build system (`bootstrap`), and
the `rust-lang/rust` CI. I guess I'm also involved in a lot of firefighting,
from CI problems to compiler beta regressions. And your usual maintenance
activities, like triaging, reviewing release notes, prioritizing regressions,
updating contribution docs, etc.

During this year I became employed full-time, and so I contribute during my free
time, which means I have less bandwidth than I used to. My contributions mostly
then manifests in helping with review bandwidth around the compiler, bootstrap
and infra parts of the Rust project, among [other
things](https://rust-lang.org/governance/people/jieyouxu/).

If I had to summarize, my main contributions would be:

- Getting rid of the `Makefile`-based `tests/run-make` test infra, in favor of [plain Rust test programs](https://github.com/rust-lang/rust/pull/136581).
- [`rust-lang/rust`](https://github.com/rust-lang/rust) CI firefighting. E.g. [(1)](https://github.com/rust-lang/rust/pull/137788) [(2)](https://github.com/rust-lang/cargo/pull/15245) [(3)](https://github.com/rust-lang/rust/pull/138690/) [(4)](https://github.com/rust-lang/rust/pull/141023), etc.
- Helped with the [`bootstrap` stage 0 sequence
  redesign](https://blog.rust-lang.org/inside-rust/2025/05/29/redesigning-the-initial-bootstrap-sequence/)
  efforts and follow-up fixes to get it over the line.
- A bunch of `compiletest` (test infra) related fixes/cleanups.

# Thoughts?

- There are way more stuff I would like to work on than I have time for, and
  said list of things keep on growing. I keep getting distracted while being
  already distracted[^distracted].
- Current full-time `$job` + free-time OSS contribution model probably works
  best for me, even though I am very glad to see initiatives like the [Rust
  Foundation Maintainers
  Fund](https://rustfoundation.org/media/announcing-the-rust-foundation-maintainers-fund/)
  to better support other maintainers. Reason is simple: I would like my hobby
  to remain my hobby, and turning it into a job risks taking away some of the
  fun.
- It's fun to interact with other maintainers from all around the world :)

---

[^review-note]: At least in `rust-lang/rust`, the PR assignee is not necessarily
    the reviewer(s) (the bors `r+` approval statistics would probably be more
    accurate.)

[^vibes]: E.g. day of week, temperature during the morning, or you know, if I
    feel like it.

[^distracted]: You can tell from my contributions already :D
