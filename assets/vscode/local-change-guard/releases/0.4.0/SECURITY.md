# Security Policy

## Supported versions

Only the latest Marketplace or GitHub release receives security fixes. The `development` branch is development code and may change without notice; `production` contains release-ready code.

## Reporting a vulnerability

Do not open a public issue for a suspected vulnerability. Email `oxara.dev@gmail.com` with:

- the affected version;
- reproduction steps or a proof of concept;
- the expected impact;
- any suggested mitigation.

Please avoid including real repository contents, credentials, private paths, or personal data. You should receive an acknowledgement within seven calendar days. We will coordinate validation, remediation, and disclosure with the reporter.

## Scope notes

Local Change Guard invokes the local `git` executable, reads worktree diffs, applies explicitly confirmed index operations, and stores classification metadata under Git's metadata directory. Reports involving unexpected working-tree mutation, command injection, path escape, unsafe worktree creation, or Webview message validation are security relevant.
