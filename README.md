# renovate-config

Shared Renovate preset for vu1n repos. Opt a repo in with a `renovate.json` of:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>vu1n/renovate-config"]
}
```

Policy (`default.json`): routine major/minor/patch bumps are off; Action SHA pins, image digest
pins/refresh and CVE fixes open PRs, gated by a minimum release age (7 days, 14 for majors, 3 for CVE
fixes). The repo is public because public repos cannot read a preset from a private one.
