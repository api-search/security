---
api_specs:
- filename: gameye-session-openapi.yml
  format: yaml
  label: Gameye Session API
  slug: gameye-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameye/refs/heads/main/openapi/gameye-session-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gameye.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: gameye.net
  spf: false
hosts:
- cert_expires: Sep 29 17:16:20 2026 GMT
  host: gameye.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 13:37:04 2026 GMT
  host: api.sandbox-gameye.gameye.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 11:50:18 2026 GMT
  host: api.production-gameye.gameye.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gameye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gameye, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gameye
provider_slug: gameye
slug: gameye-domain-security
source_filename: gameye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gameye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:16:20 2026 GMT\n  hsts: false\n- host: api.sandbox-gameye.gameye.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 13:37:04 2026 GMT\n  hsts: null\n- host: api.production-gameye.gameye.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:50:18 2026 GMT\n  hsts: null\ndomains:\n- domain: gameye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gameye.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameye/refs/heads/main/security/gameye-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Game Server Hosting
- Game Server Orchestration
- Multiplayer
- Containers
- Infrastructure
- Gaming
- Edge Computing
- DevOps
---
