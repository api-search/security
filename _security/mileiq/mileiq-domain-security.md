---
api_specs:
- filename: mileiq-external-openapi-original.json
  format: json
  label: MileIQ External API
  slug: mileiq-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mileiq/refs/heads/main/openapi/mileiq-external-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mileiq.com
  spf: true
hosts:
- cert_expires: Sep 16 15:07:31 2026 GMT
  host: www.mileiq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 08:53:36 2026 GMT
  host: developer.mileiq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 08:53:36 2026 GMT
  host: external-api.mileiq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mileiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MileIQ, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MileIQ
provider_slug: mileiq
slug: mileiq-domain-security
source_filename: mileiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mileiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:07:31 2026 GMT\n  hsts: false\n- host: developer.mileiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 08:53:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: external-api.mileiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 08:53:36 2026 GMT\n  hsts: null\ndomains:\n- domain: mileiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mileiq/refs/heads/main/security/mileiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Mileage Tracking
- Expense Management
- Transportation
- Tax
- Accounting
- Location
- Fleet
---
