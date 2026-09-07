---
api_specs:
- filename: openapi.json
  format: json
  label: Grade API
  slug: grade-api
  spec_type: OpenAPI
  url: https://gradetv.net/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gradetv.net
  spf: true
hosts:
- cert_expires: Nov 11 19:43:14 2026 GMT
  host: gradetv.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gradetv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Grade
provider_slug: gradetv
slug: gradetv-domain-security
source_filename: gradetv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gradetv.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 19:43:14 2026 GMT\n  hsts: false\ndomains:\n- domain: gradetv.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradetv/refs/heads/main/security/gradetv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- IPTV
- Streaming
- Live TV
- Live Radio
- Media Catalog
- Broadcast Metadata
- EPG
- TV Guide
- Content Aggregation
- Agent-native
- MCP
- x402
- Micropayments
- Brazil
---
