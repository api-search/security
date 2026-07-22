---
api_specs:
- filename: forum-openapi-original.yml
  format: yaml
  label: Forum API
  slug: forum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forum/refs/heads/main/openapi/forum-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: forum.market
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.forum.market
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Forum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forum
provider_slug: forum
slug: forum-domain-security
source_filename: forum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.forum.market\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: forum.market\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forum/refs/heads/main/security/forum-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Trading
- Exchange
- Perpetual Futures
- Market Data
- Attention Economy
- Fintech
- WebSocket
- Real Time
---
