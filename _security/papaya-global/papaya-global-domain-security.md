---
api_specs:
- filename: papaya-global-workforce-payments-api.yml
  format: yaml
  label: Papaya Global Workforce Payments API
  slug: workforce-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papaya-global/refs/heads/main/openapi/papaya-global-workforce-payments-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: papayaglobal.com
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.papayaglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 01:01:22 2026 GMT
  host: docs.papayaglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.papayaglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Papaya Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Papaya Global, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Papaya Global
provider_slug: papaya-global
slug: papaya-global-domain-security
source_filename: papaya-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.papayaglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: null\n- host: docs.papayaglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:01:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.papayaglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: papayaglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/papaya-global/refs/heads/main/security/papaya-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payroll
- Global Workforce
- HR
- Payments
- Employer of Record
- Contractor Management
- Compliance
---
