---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: replay.io
  spf: true
hosts:
- cert_expires: Sep 12 09:00:48 2026 GMT
  host: www.replay.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 01:55:23 2026 GMT
  host: docs.replay.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:34:44 2026 GMT
  host: api.replay.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Replay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Replay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Replay
provider_slug: replay
slug: replay-domain-security
source_filename: replay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.replay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 09:00:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.replay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 01:55:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.replay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:34:44 2026 GMT\n  hsts: null\ndomains:\n- domain: replay.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replay/refs/heads/main/security/replay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Debugging
- Testing
- Quality Assurance
- Developer Tools
- Time Travel Debugging
- MCP
- GraphQL
- Browser Automation
- AI
---
