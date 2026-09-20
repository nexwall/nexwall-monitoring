# Nexwall Monitoring

Monitoring services for Nexwall Firewall, written in Go.

| Binary | Purpose |
|---|---|
| `ns-flows` | Reads network flows from the traffic classification service, keeps the active flows in memory and serves them through a paginated REST API on a Unix socket |
| `ns-stats` | Keeps traffic statistics in a SQLite database, resolves remote hosts with reverse DNS, exports hourly statistics and serves them through a local HTTP API |

Both are installed on the firewall and consumed by the web interface.

## License

GPL-3.0-only, see `LICENSE`. Attribution and the list of changes are in `NOTICE.md`.
