---
api_specs:
- filename: monid-openapi.json
  format: json
  label: Monid API
  slug: monid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: monid.ai
  spf: false
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: monid.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Monid
provider_slug: monid
slug: monid-domain-security
source_filename: monid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: monid.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/security/monid-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Agents
- MCP
- Tools
- Data
- API Marketplace
---
