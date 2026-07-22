---
api_specs:
- filename: parcha-openapi-original.json
  format: json
  label: Parcha API
  slug: parcha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcha/refs/heads/main/openapi/parcha-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parcha.ai
  spf: true
hosts:
- cert_expires: Aug  3 11:12:02 2026 GMT
  host: www.parcha.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 17:05:59 2026 GMT
  host: api.parcha.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: demo.parcha.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Parcha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parcha, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parcha
provider_slug: parcha
slug: parcha-domain-security
source_filename: parcha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parcha.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 11:12:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.parcha.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:05:59 2026 GMT\n  hsts: null\n- host: demo.parcha.ai\n  https: false\ndomains:\n- domain: parcha.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parcha/refs/heads/main/security/parcha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Compliance
- KYB
- KYC
- Due Diligence
- AML
- Sanctions Screening
- Identity Verification
- Financial Services
- Artificial Intelligence
---
