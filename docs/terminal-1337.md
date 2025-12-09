# terminal-1337

Modern CLI tools that replace legacy Unix utilities.

## Tools

| Legacy | Elite | Why |
|--------|-------|-----|
| grep | ripgrep (rg) | 10x faster, respects .gitignore |
| find | fd | Simpler syntax, faster |
| cat | bat | Syntax highlighting, line numbers |
| ls | eza | Git status, icons |
| curl | xh | Cleaner output, sensible defaults |
| history | atuin | Searchable, synced across machines |
| - | fzf | Fuzzy finder for everything |
| - | jq | JSON processing |

## How It Works

1. Detects installed tools
2. Uses elite tools when available
3. Offers to install missing ones
4. Falls back to standard tools if declined

## Examples

```bash
# Search code
rg "TODO"                    # vs grep -r "TODO" .

# Find files
fd -e ts                     # vs find . -name "*.ts"

# View file
bat config.json              # vs cat config.json

# List directory
eza -la --git                # vs ls -la
```

## Reference Files

Each tool has comprehensive docs in `plugins/terminal-1337/skills/references/`:

```
ripgrep.md, fd.md, bat.md, eza.md, fzf.md, xh.md, jq.md, atuin.md
```

## Triggers

Activates when Claude needs to:
- Search code or files
- View file contents
- List directories
- Make HTTP requests
- Process JSON
