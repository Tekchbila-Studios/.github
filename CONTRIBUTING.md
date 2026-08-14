# Contributing

Thanks for taking the time. This is a small studio, so here is exactly what
happens to a contribution and what makes one easy to merge.

## Before you write code

**Open an issue first for anything non-trivial.** A typo fix or an obviously
correct one-line bug fix can go straight to a pull request. Anything that adds a
feature, changes behaviour, or touches an interface deserves a short issue first
— it costs you ten minutes and can save you a rejected afternoon.

If an issue already exists, say you're picking it up so nobody duplicates the
work.

## Pull requests

- **One change per pull request.** A refactor bundled with a bug fix is two
  reviews wearing a trenchcoat, and the bug fix waits for the refactor.
- **Explain the *why* in the description.** The diff already shows what changed.
  What it can't show is the reasoning, the alternative you rejected, or the
  constraint that made the obvious approach wrong.
- **Include a test** when you fix a bug. A test that fails before your change
  and passes after it is the only durable proof the bug is gone.
- **Match the surrounding code.** Naming, comment density, error handling — a
  patch that reads like the file it lands in needs no style debate.
- **Keep the branch current** with `main`, and let it be squash-merged. Every
  repo here squashes; you don't need to tidy your intermediate commits.

## Commit messages

Conventional Commits, present tense, and the body explains why:

```
fix: strip provider aliases from plan output before upload

Aliased providers carried their config through to the diagram payload,
which for the vault provider meant the token was included verbatim.
```

## Review

You'll get a first response within a few days. Review comments are about the
code, never about you — and if a comment reads harsher than intended, assume
brevity rather than hostility and push back.

Not every good pull request gets merged. Sometimes it's the right change at the
wrong time, or it commits us to something we're not ready to support. If that
happens we'll say so plainly and explain why, rather than letting it sit.

## Reporting security issues

Not here. See [SECURITY.md](SECURITY.md) — never in a public issue or pull
request.

## Conduct

By participating you agree to the [Code of Conduct](CODE_OF_CONDUCT.md).
