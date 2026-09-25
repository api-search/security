---
api_specs:
- filename: rsperformance-online-ai-gateway-openapi.yml
  format: yaml
  label: RS Performance AI Gateway API
  slug: rs-performance-ai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsperformance-online/refs/heads/main/openapi/rsperformance-online-ai-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rsperformance.online
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rs3d.pl
  spf: true
hosts:
- cert_expires: Dec 13 20:14:33 2026 GMT
  host: rsperformance.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 16:52:26 2026 GMT
  host: ai.rsperformance.online
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 19:50:32 2026 GMT
  host: mcp.rs3d.pl
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Rsperformance Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RS Performance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RS Performance
provider_slug: rsperformance-online
slug: rsperformance-online-domain-security
source_filename: rsperformance-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rsperformance.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 20:14:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ai.rsperformance.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 16:52:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.rs3d.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 19:50:32 2026 GMT\n  hsts: null\ndomains:\n- domain: rsperformance.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rs3d.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rsperformance-online/refs/heads/main/security/rsperformance-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Auto Repair
- Vehicle Diagnostics
- OBD-II
- Fault Codes
- Knowledge Base
- Semantic Search
- A2A
- MCP
- Agent-Native
- Local Business
- Poland
---
