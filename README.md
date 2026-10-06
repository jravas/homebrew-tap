# jravas/homebrew-tap

Homebrew tap for apps by Josip Ravas.

```bash
brew tap jravas/tap
brew install --cask claude-storage-cleaner
xattr -dr com.apple.quarantine "/Applications/Claude Storage Cleaner.app"
```

| Cask                     | What it is                                                                 |
| ------------------------ | -------------------------------------------------------------------------- |
| `claude-storage-cleaner` | [See where Claude Code's disk usage goes and clean it up safely](https://github.com/jravas/calude-storage-cleaner) |

The `xattr` line is needed because the app is not yet signed with an Apple
Developer ID, and Homebrew 5 no longer offers `--no-quarantine`.
