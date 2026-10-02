# GitHub520 — English Guide

A hosts-file data project intended to improve access to GitHub-related domains. This fork contains generated hosts snapshots, a Python refresh script, a README template, and update workflows.

## Requirements

No application installation is needed to inspect the data. Updating the data uses Python and the declared requirements; applying it needs OS administrator access.

## Getting started

Read `hosts` and `hosts.json`, compare their timestamp with the present date, and back up your OS hosts file before any manual changes. The checked-in snapshot is historical and must not be assumed current.

## Project structure

| Path | Purpose |
| --- | --- |
| `hosts` | Generated hostname/address snapshot |
| `hosts.json` | JSON snapshot |
| `fetch_ips.py` | Data refresh script |
| `requirements.txt` | Refresh dependencies |
| `README_template.md` | Template used to regenerate the main README |
| `.github` | Automated update workflow |

## Configuration and limitations

The original Chinese README contains platform-specific instructions and screenshots. Stale IP overrides can break connectivity; remove obsolete entries rather than disabling TLS verification. Hosts overrides do not replace network-policy authorization.

## Development and validation

For development, use `python -m pip install -r requirements.txt` and inspect the refresh script/workflow before executing it, because it updates generated files. Check hostname resolution and HTTPS certificate validation after any authorized local hosts changes.

## Related projects and attribution

Original project: [521xueweihan/GitHub520](https://github.com/521xueweihan/GitHub520). Preserve its CC BY-NC-ND 4.0 notices and attribution.

## License

The original documentation declares CC BY-NC-ND 4.0; see the notices in [README.md](README.md). This guide does not replace those terms.
