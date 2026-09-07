# SDODS Homebrew tap

```bash
brew install siri1410/sdods/sdods
```

BDD test automation for UI, API and hybrid flows — <https://sdods.com>.

The formula installs the published `@sdods/cli` package against Homebrew's `node`, rather than
vendoring a second Node runtime. Browser engines are a separate download, because most API suites
never need one:

```bash
sdods browsers install chromium
```

## This repository holds the formula only

`Formula/sdods.rb` is generated in the SDODS repository by `scripts/sync-channels.ts`, which
computes the `sha256` from the npm tarball it downloads. Do not edit it here — a hand-edited
formula is one that drifts from the release it claims to install.
