---
api_specs:
- filename: openapi.json
  format: json
  label: FluentEDI Tools API
  slug: fluentedi-tools-api
  spec_type: OpenAPI
  url: https://fluentedi.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: fluentedi.com
  spf: false
hosts:
- cert_expires: Oct 17 16:51:25 2026 GMT
  host: fluentedi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fluentedi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FluentEDI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: FluentEDI
provider_slug: fluentedi
slug: fluentedi-domain-security
source_filename: fluentedi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluentedi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 16:51:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fluentedi.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/security/fluentedi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- EDI
- X12
- Retail EDI
- AI Agents
- MCP
- Developer Tools
- JSON
- Cryptography
- Data Validation
- Supply Chain
---
