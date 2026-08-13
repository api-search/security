---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: valid.co
  spf: true
hosts:
- cert_expires: Nov  1 11:09:55 2026 GMT
  host: valid.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 15:31:09 2026 GMT
  host: mcp.valid.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valid, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Valid
provider_slug: valid
slug: valid-domain-security
source_filename: valid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valid.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 11:09:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.valid.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:31:09 2026 GMT\n  hsts: null\ndomains:\n- domain: valid.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valid/refs/heads/main/security/valid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Marketing
- Artificial Intelligence
- Creative
- Media Buying
- Influencers
- MCP
- Agents
- Performance Marketing
---
