# Demo repo for renovatebot/renovate#14828

see https://github.com/renovatebot/renovate/issues/14828

steps to reproduce

```json
export RENOVATE_TOKEN=xxx
export RENOVATE_EXTENDS=hojerst/renovate-issue-14828
renovate --dry-run=true hojerst/renovate-issue-14828
```

Note: it works completely fine, when this `extends` block is used inside an global config.js or repository. It seems to
break ONLY when used with `RENOVATE_EXTENDS` env var.
