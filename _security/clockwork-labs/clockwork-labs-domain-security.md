---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spacetimedb.com
  spf: false
hosts:
- cert_expires: Oct  2 03:25:11 2026 GMT
  host: spacetimedb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 16:11:34 2026 GMT
  host: maincloud.spacetimedb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clockwork Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clockwork Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Clockwork Labs
provider_slug: clockwork-labs
slug: clockwork-labs-domain-security
source_filename: clockwork-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spacetimedb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:25:11 2026 GMT\n  hsts: false\n- host: maincloud.spacetimedb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:11:34 2026 GMT\n  hsts: null\ndomains:\n- domain: spacetimedb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clockwork-labs/refs/heads/main/security/clockwork-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Database
- Real-Time
- WebSocket
- Game Backend
- Multiplayer
- Serverless
- WebAssembly
- Developer Tools
- Infrastructure
---
