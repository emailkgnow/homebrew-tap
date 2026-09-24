# emailkgnow/tap

Homebrew formulae by [emailkgnow](https://github.com/emailkgnow).

## bt (Bullet Terminal)

A terminal life manager built on four bullets: tasks, notes, journals and events, stored as plain Markdown. See [bullet-terminal](https://github.com/emailkgnow/bullet-terminal).

```bash
brew install emailkgnow/tap/bullet-terminal
bt init
```

Upgrade with `brew upgrade bullet-terminal`. Your config (`~/.config/bt/`) and data (`~/bullet-terminal/` by default) are never touched by upgrades or `brew uninstall`.

## How releases reach this tap

The `brew bump` workflow checks bullet-terminal's GitHub releases daily (or on demand: `gh workflow run autobump.yml -R emailkgnow/homebrew-tap`) and opens a pull request when a new version is tagged. `brew test-bot` builds and tests it on macOS and Linux. Once green, publish it with prebuilt bottles via `gh workflow run publish.yml -R emailkgnow/homebrew-tap -f pull_request=<number>`, or simply merge the PR (users then build from source).
