---
api_specs:
- filename: tesser-openapi-original.json
  format: json
  label: Tesser API
  slug: tesser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/openapi/tesser-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tesser.xyz
  spf: true
hosts:
- cert_expires: Oct  1 09:16:07 2026 GMT
  host: tesser.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 01:28:47 2026 GMT
  host: docs.tesser.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 05:41:20 2026 GMT
  host: api.tesser.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tesser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tesser, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tesser
provider_slug: tesser
slug: tesser-domain-security
source_filename: tesser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tesser.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tesser.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:28:47 2026 GMT\n  hsts: false\n- host: api.tesser.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:41:20 2026 GMT\n  hsts: null\ndomains:\n- domain: tesser.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesser/refs/heads/main/security/tesser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Stablecoins
- Cross-Border Payments
- Fintech
- Treasury
- Banking
- Blockchain
- Compliance
- MCP
- Developer Platform
---
