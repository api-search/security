---
api_specs:
- filename: datanomik-openbanking-openapi.json
  format: json
  label: Datanomik OpenBanking API
  slug: datanomik-openbanking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-openbanking-openapi.json
- filename: datanomik-remuneration-openapi.json
  format: json
  label: Datanomik Treasury / Remuneration API
  slug: datanomik-treasury-remuneration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/openapi/datanomik-remuneration-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: datanomik.com
  spf: true
hosts:
- cert_expires: Sep 20 04:08:43 2026 GMT
  host: datanomik.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 16:15:43 2026 GMT
  host: docs.datanomik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: api.datanomik.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datanomik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datanomik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Datanomik
provider_slug: datanomik
slug: datanomik-domain-security
source_filename: datanomik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datanomik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:08:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.datanomik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:15:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.datanomik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datanomik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datanomik/refs/heads/main/security/datanomik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Open Finance
- Open Banking
- Treasury Management
- Cash Management
- Payments
- PIX
- Financial Data
- Bank Connectivity
- Brazil
- LatAm
- Fintech
---
