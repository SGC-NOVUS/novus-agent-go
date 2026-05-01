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

## Security
Use signed release artifacts and rotate secrets according to policy.

## License
See LICENSE in this repository.
