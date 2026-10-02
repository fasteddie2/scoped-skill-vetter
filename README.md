# Scoped skill vetter

An instructions-only skill for reviewing third-party agent skills before an
authorized installation. It evaluates actual behavior and permissions, reports
unreviewed dependencies explicitly, and avoids treating popularity as proof of
safety. It is not a malware scanner or a sandbox.

## Use

Copy this repository into a folder named `scoped-skill-vetter` under your agent's
configured skill directory. Follow that agent's supported registration/discovery
process. Confirm in a fresh session that it reads `SKILL.md`; file presence alone
does not establish activation. No hooks or dependencies are included.

Example: "Use scoped-skill-vetter to review this candidate folder. Do not execute
its scripts. Identify the exact files inspected, missing coverage, requested
permissions, and your verdict."

The procedure preserves an existing installation request; it does not require
repeated approval for routine authorized steps or bypass platform approvals.
Review updates separately. Remove only this skill directory to uninstall; retain
any review reports as user data. Do not publish real reports without sanitizing them.

## Attribution

Adapted from [spclaudehome/skill-vetter v1.0.0](https://clawhub.ai/spclaudehome/skills/skill-vetter),
whose listing specifies MIT-0. This is an independent adaptation, not an official
upstream release or endorsement. Changes include purpose-based permission review,
explicit incomplete coverage, platform checks, and scoped authorization. The
upstream executable payload and future releases are not certified by this package.

License: MIT-0; see `LICENSE`. This repository contains no personal configuration,
logs, credentials, or production review records. See `VALIDATION.md` for limits.
