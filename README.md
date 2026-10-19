# maser-cli

`registry.json` is the registry the Maser harness CLI reads to check task repos and find its current release.

- `task_repos` is regenerated hourly by the `registry` workflow in `maser-harnesses`. Don't edit it by hand.
- `cli` is set by each release: `current`, `min_version`, and the SHA-256 of every platform's binary. The CLI refuses to install a binary that doesn't match.

Every released CLI has `https://raw.githubusercontent.com/handshake-project-maser/maser-cli/main/registry.json` built in, so don't rename the repo, the `main` branch or the file.
