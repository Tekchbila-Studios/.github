# Security Policy

## Reporting a vulnerability

**Do not open a public issue.** A public report is a public exploit for however
long it takes to ship a fix.

Two ways to reach us, either is fine:

- **Preferred** — the *Report a vulnerability* button under the **Security** tab
  of the affected repository. This opens a private advisory that only the
  maintainers can see, and it keeps the discussion attached to the code.
- **Email** — <contact@infragr.am>. Put "security" in the subject line so it
  gets triaged ahead of everything else in that inbox.

Please include:

- what the issue is, and which repository or which part of Infragr.am it affects
- the steps to reproduce it, or a proof of concept
- what an attacker gets out of it — that is what decides how fast we move

## What to expect

| | |
|---|---|
| First response | Within 3 business days |
| Assessment and severity | Within 7 days of that response |
| Fix or mitigation | As fast as the severity warrants; we will tell you the target date rather than leave you guessing |

This is a small studio, not a 24/7 security team. We would rather commit to
dates we can hold than publish a one-hour SLA we cannot.

We will credit you in the advisory unless you would prefer we didn't — say so
in your report.

## Scope

In scope: anything in this organization's repositories, and the Infragr.am
service at <https://infragr.am>.

Particularly interested in: anything where a customer's Terraform plan, state,
or credentials could leak. Infragr.am's core promise is that secrets are
stripped before a plan leaves your runner, so a hole in that path is the most
serious class of bug we can have.

Out of scope: findings from automated scanners with no demonstrated impact,
missing security headers with no exploit path, denial of service by volume, and
social engineering of studio staff.

## Please don't

Access, modify, or exfiltrate data that isn't yours; degrade the service for
other users; or run automated scans heavy enough to look like an attack. Testing
against your own account and your own data is always fine.
