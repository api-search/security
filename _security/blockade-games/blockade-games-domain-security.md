---
api_specs:
- filename: blockade-games-skybox-openapi.yml
  format: yaml
  label: Skybox AI API
  slug: skybox-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockade-games/refs/heads/main/openapi/blockade-games-skybox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blockade.games
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blockadelabs.com
  spf: true
hosts:
- cert_expires: Oct  6 18:47:53 2026 GMT
  host: blockade.games
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: backend.blockadelabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockade Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockade Games, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Blockade Games
provider_slug: blockade-games
slug: blockade-games-domain-security
source_filename: blockade-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockade.games\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 18:47:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: backend.blockadelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: blockade.games\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: blockadelabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockade-games/refs/heads/main/security/blockade-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Image Generation
- 3D
- Gaming
- Virtual Reality
- Content Generation
- Skybox
---
