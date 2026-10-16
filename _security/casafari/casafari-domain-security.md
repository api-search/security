---
api_specs:
- filename: casafari-api-openapi.json
  format: json
  label: Casafari API API
  slug: casafari-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casafari/refs/heads/main/openapi/_original/casafari-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: casafari.com
  spf: true
hosts:
- cert_expires: Nov 22 07:33:24 2026 GMT
  host: www.casafari.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Casafari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Casafari API and MCP Platform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Casafari API and MCP Platform
provider_slug: casafari
slug: casafari-domain-security
source_filename: casafari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.casafari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 07:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: casafari.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casafari/refs/heads/main/security/casafari-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate Data
- Property Sourcing
- Valuation
- Market Analytics
- API
- CRM
- Real Estate Software
---
