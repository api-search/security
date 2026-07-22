---
api_specs:
- filename: omni-openapi-original.yml
  format: yaml
  label: Omni API
  slug: omni-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omni/refs/heads/main/openapi/omni-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: omni.co
  spf: true
hosts:
- cert_expires: Oct  3 17:43:58 2026 GMT
  host: omni.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Omni
provider_slug: omni
slug: omni-domain-security
source_filename: omni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omni.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:43:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: omni.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omni/refs/heads/main/security/omni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Analytics
- Business Intelligence
- Data
- Embedded Analytics
- Semantic Layer
- MCP
---
