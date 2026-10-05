# AKA Security Scoop bucket

[Scoop](https://scoop.sh) manifests for [AKA Security](https://akasecurity.io) tools on Windows.

```powershell
scoop bucket add akasecurity https://github.com/akasecurity/scoop-bucket
scoop install aka
```

## Manifests

- **[aka](https://github.com/akasecurity/ai-tc)** — the `aka` CLI for AI Traffic Control, a
  local-first security control plane for AI coding agents. A self-contained binary with its own
  runtime; no Node.js required. Windows x64. Run `aka init` after installing, and
  `scoop update aka` to upgrade.

`bucket/aka.json` is written by the ai-tc release workflow, not by hand: every `bin-v*` release
renders it from its own `SHA256SUMS` and commits it here. Do not hand-edit it — the next release
overwrites the file. The same manifest is attached to each release, so
`scoop install https://github.com/akasecurity/ai-tc/releases/download/bin-latest/aka.json` also
works without adding this bucket.

Each manifest installs its upstream project under that project's own license.
<https://akasecurity.io>
