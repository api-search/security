---
api_specs:
- filename: pigment-external-api-openapi.json
  format: json
  label: Pigment External API
  slug: pigment-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/openapi/pigment-external-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pigment.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pigment.app
  spf: true
hosts:
- cert_expires: Oct  3 06:56:35 2026 GMT
  host: www.pigment.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 14:00:41 2026 GMT
  host: kb.pigment.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 09:50:25 2026 GMT
  host: pigment.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pigment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pigment, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pigment
provider_slug: pigment
slug: pigment-domain-security
source_filename: pigment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pigment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:56:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kb.pigment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 14:00:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pigment.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:50:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pigment.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pigment.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pigment/refs/heads/main/security/pigment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Software
- Business Planning
- Financial Planning
- FP&A
- Analytics
- EPM
- Data Integration
- MCP
- SCIM
---
