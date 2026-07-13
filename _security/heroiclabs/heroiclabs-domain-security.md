---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Nakama API
  slug: nakama-api
  spec_type: OpenAPI
  url: https://heroiclabs.github.io/nakama-docs/
- filename: heroiclabs-hiro-rpc-api-openapi.yml
  format: yaml
  label: Hiro RPC API
  slug: hiro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroiclabs/refs/heads/main/openapi/heroiclabs-hiro-rpc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: heroiclabs.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: heroiclabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
- host: api.heroiclabs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Heroiclabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heroic Labs, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Heroic Labs
provider_slug: heroiclabs
slug: heroiclabs-domain-security
source_filename: heroiclabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heroiclabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n- host: 127.0.0.1\n  https: false\n- host: api.heroiclabs.com\n  https: false\ndomains:\n- domain: heroiclabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroiclabs/refs/heads/main/security/heroiclabs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Game Backend
- Multiplayer
- Real-Time
- WebSocket
- Matchmaking
- Leaderboards
- Social Gaming
- Open Source
- LiveOps
- gRPC
---
