---
api_specs:
- filename: highline-fi-openapi.yml
  format: yaml
  label: Highline Pay by Paycheck API
  slug: pay-by-paycheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/openapi/highline-fi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: highline.co
  spf: true
hosts:
- cert_expires: Aug 27 09:54:55 2026 GMT
  host: highline.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 07:32:45 2026 GMT
  host: docs.highline.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 09:54:55 2026 GMT
  host: api.highline.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Highline Fi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highline, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Highline
provider_slug: highline-fi
slug: highline-fi-domain-security
source_filename: highline-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highline.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:54:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.highline.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:32:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.highline.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:54:55 2026 GMT\n  hsts: null\ndomains:\n- domain: highline.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highline-fi/refs/heads/main/security/highline-fi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embedded Finance
- Payroll
- Payments
- ACH
- Bill Pay
- Lending
- Direct Deposit
- API-First
- Webhooks
- Pay by Paycheck
---
