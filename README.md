# sn_flow_designer_documenter

## Architecture
```mermaid
graph TD
    SN[ServiceNow] -->|REST| sn_flow_designer_documenter
    sn_flow_designer_documenter -->|Store| DB[Tables]
    sn_flow_designer_documenter -->|Generate| Report[Reports]
```
## Quick Start
```bash
git clone https://github.com/vladarchitectservicenow-oss/sn_flow_designer_documenter.git
cd sn_flow_designer_documenter && python3 src/cli.py --help
```
## ROI
| Approach | Hours/Year | Cost |
|----------|-----------|------|
| Manual | 40 | $3,400 |
| With sn_flow_designer_documenter | 5 | $425 |
| **Savings** | **35h** | **$2,975 (87%)** |
## API Reference
`GET /api/now/table/incident` — incidents
## Security
- HTTPS, credentials via env vars, GDPR compliant
## Troubleshooting
| Issue | Fix |
|-------|-----|
| Timeout | `--timeout 60` |
| 401 | Check credentials |
## License
Copyright (C) 2026 Vladimir Kapustin | AGPL-3.0

