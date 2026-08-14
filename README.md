# .github

The public face of Tekchbila Studios, and the org's shared boilerplate. No code.

| Path | What it does |
|---|---|
| `profile/README.md` | Renders as <https://github.com/Tekchbila-Studios> |
| `CONTRIBUTING.md`, `SECURITY.md`, `SUPPORT.md`, `CODE_OF_CONDUCT.md` | Used by **every** repo in the org — public and private — that has no copy of its own |
| `.github/ISSUE_TEMPLATE/`, `.github/PULL_REQUEST_TEMPLATE.md` | Default issue and pull request templates for those same repos |

A repository always wins over the defaults: GitHub looks in that repo's
`.github` folder, then its root, then its `docs` folder, and only then here.

One override rule is all-or-nothing — if a repo has **any** file in its own
`.github/ISSUE_TEMPLATE`, none of this repo's issue templates apply to it.

This repo is public because it has to be. GitHub does not read defaults from a
private `.github` repo, and there is no private counterpart. Publishing the
boilerplate is what lets the org's private repositories inherit it.

## This repo is generated

Every file here is written by Terraform from
[`source-management`](https://github.com/Tekchbila-Studios/source-management),
under `content/dot-github/`.

Editing a file through the GitHub UI appears to work and is reverted by the next
`terraform apply`. Send the change to `source-management` instead.
