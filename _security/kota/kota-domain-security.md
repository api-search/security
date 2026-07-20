---
api_specs:
- filename: kota-openapi-original.json
  format: json
  label: Kota API
  slug: kota-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kota/refs/heads/main/openapi/kota-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kota.io
  spf: true
hosts:
- cert_expires: Sep 15 18:41:18 2026 GMT
  host: www.kota.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 08:31:51 2026 GMT
  host: docs.kota.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: api.kota.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kota Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kota, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kota
provider_slug: kota
slug: kota-domain-security
source_filename: kota-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kota.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:41:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kota.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:31:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kota.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kota.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kota/refs/heads/main/security/kota-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Insurance
- Employee Benefits
- Health Insurance
- Pensions
- Insurtech
- Embedded Finance
- Human Resources
- Payroll
---
