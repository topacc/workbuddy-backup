# workbuddy-backup

Backup of selected `~/.workbuddy` content, pushed on 2026-07-18T11:35:12 (local time, Asia/Shanghai).

## Included
- `workbuddy.db` — consistent online SQLite snapshot (automations table lives here)
- `skills/` — installed skills
- `memory/` — per-user memory files
- `MEMORY.md` — top-level user memory
- `.mcp.json` — MCP server config (verified: no embedded secrets)
- `settings.json` — app settings (verified: no embedded secrets, only a user UUID)

## Not included (intentional)
- `mcp.json` — does not exist (only `.mcp.json` exists)
- `automations/` — not a folder; automations stored inside `workbuddy.db`
- `experts/` — no top-level dir; `app/cache/experts` is regenerable marketplace catalog, skipped
- `workbuddy.db-wal` / `workbuddy.db-shm` — volatile; folded into the consistent db snapshot
- runtime data: sessions/, traces/, logs/, binaries/, connectors state, etc.

## Restore hint
Copy these items back to `~/.workbuddy/` (close the WorkBuddy app first, especially before replacing `workbuddy.db`).

See `BACKUP_INFO.json` for the full manifest with table row counts.
