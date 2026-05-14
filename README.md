# NOVUS-OS Agent
![NOVUS-OS Banner](ссылка_на_красивую_картинку_с_логотипом)

Official high-performance daemon for game server and node management.

## Repository Role
Public release channel for NOVUS-OS Agent binaries, installer artifacts, and operator documentation.

## Build Origin
Private source repository: SGC-NOVUS/agent-core.

## Release Flow
1. Development is performed in SGC-NOVUS/agent-core.
2. CI/CD builds versioned agent artifacts.
3. Release is published to SGC-NOVUS/agent.

## Integration
NOVUS-OS Panel communicates with Agent using authenticated HTTP APIs.

## Install

Latest public releases publish these canonical assets:

- `novus-agent-linux-amd64`
- `novus-agent-linux-arm64`
- `install-novus-agent.sh`

Example install flow:

```bash
PANEL_URL=https://panel.example.com \
PANEL_TOKEN=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9... \
AGENT_SHARED_SECRET=change-me \
AGENT_ID=agent-01 \
bash <(curl -fsSL https://github.com/SGC-NOVUS/agent/releases/download/vX.Y.Z/install-novus-agent.sh)
systemctl enable --now novus-agent
```

## Security
Use signed release artifacts and rotate secrets according to policy.

## License
See LICENSE in this repository.
