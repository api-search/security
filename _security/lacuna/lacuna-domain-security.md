---
api_specs:
- filename: lacuna-lacuna-music-api-api-openapi.yml
  format: yaml
  label: Lacuna Lacuna Music API API
  slug: lacuna-lacuna-music-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/openapi/lacuna-lacuna-music-api-api-openapi.yml
- filename: lacuna-music-api-openapi.yml
  format: yaml
  label: Lacuna Music API
  slug: lacuna-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/openapi/lacuna-music-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lacuna.fm
  spf: true
hosts:
- cert_expires: Nov  4 09:49:55 2026 GMT
  host: www.lacuna.fm
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lacuna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lacuna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lacuna
provider_slug: lacuna
slug: lacuna-domain-security
source_filename: lacuna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lacuna.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 09:49:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lacuna.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/security/lacuna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Music
- Music Generation
- AI Song Generator
- AI Lyrics Generator
- Audio
- MIDI
- Songwriting
- Generative AI
- MCP Server
- AgentSkill
- A2A
- Developer Tools
---
