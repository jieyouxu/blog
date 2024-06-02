+++
title = "A ferrisClueless reviewer"
date = 2024-06-02
description = "My experiences being on the rust compiler review rotation for the first time"
[taxonomies]
tags = ["rustc", "code-review", "compiler", "rust"]
+++

In this post, I describe my experiences being on the Rust compiler [`rustc`]'s review rotation for
the first time, so far.

## Background

### Pull requests to [`rustc`] and code reviews

[`rustc`] is maintained by the [compiler team] ("T-compiler"). Pull requests (PRs) to the compiler
are expected to go through code reviews and requires approval from an authorized reviewer before the
changes can be merged to `master`. Specifically, T-compiler reviewers.

### What's the T-compiler review rotation?

The specifics are explained in more details in the [re-organize the compiler
team][compiler-reorganize] RFC, but the gist is that T-compiler members who volunteered to be on the
review rotation will be randomly assigned PRs (or explicitly requested by PR authors or others) to
review PRs primarily affecting the compiler.

## About me

I am a *very* new T-compiler contributor. I was invited to join T-compiler contributors
approximately [two months ago][compiler-invite] (at the time this blog post was written). I am new
to the compiler in general: I've only made changes to the compiler in [random PRs here and
there][my-prs]. Amusingly, looking through the PR history, many of my contributions to
[rust-lang/rust][rust] are not to the compiler itself (code in `compiler/`), but to the test
infrastructure: to the test harness `compiletest` and to the `run-make` test suite.

## Joining the compiler review rotation

As you can imagine, [`rustc`] is a big codebase, and I am not familiar with many parts of the
compiler. But that's why we have a compiler *team*: different members on the team are familiar with
different parts of the compiler.

<center>
    <figure>
        <img src="ferris_clueless.png" width=100px>
        <figcaption>`:ferrisClueless:`. Taken from the Rust community discord but I could not find the original author.</figcaption>
    </figure>
</center>


I [signed up for the compiler review rotation for the first time][rotation-signup] anyway on
2024-04-05 and have since been [assigned PRs to review][assigned-prs] (this list is not exhaustive
because I have reviewed and/or approved PRs that are not assigned to me).


[`rustc`]: https://github.com/rust-lang/rust
[rust]: https://github.com/rust-lang/rust
[compiler team]: https://www.rust-lang.org/governance/teams/compiler
[compiler-reviewers]: https://github.com/rust-lang/rust/blob/a83cf567b5949691de67f06895d9fe0404c40d27/triagebot.toml#L898-L919
[compiler-reorganize]: https://github.com/rust-lang/rfcs/pull/3599
[rotation-signup]: https://github.com/rust-lang/rust/pull/123509
[assigned-prs]: https://github.com/rust-lang/rust/pulls?q=is%3Apr+assignee%3Ajieyouxu+
[compiler-invite]: https://github.com/rust-lang/team/pull/1421
[my-prs]: https://github.com/rust-lang/rust/pulls?q=author%3Ajieyouxu+-label%3Arollup+
