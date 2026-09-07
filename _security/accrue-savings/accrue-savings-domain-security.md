---
api_specs:
- filename: accrue-savings-merchant-api-openapi.yaml
  format: yaml
  label: Accrue Merchant API
  slug: accrue-savings-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/openapi/accrue-savings-merchant-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: byaccrue.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: accruesavings.com
  spf: true
hosts:
- cert_expires: Nov 28 10:28:22 2026 GMT
  host: www.byaccrue.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 02:43:34 2026 GMT
  host: docs.byaccrue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: merchant-api.accruesavings.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Accrue Savings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accrue Savings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Accrue Savings
provider_slug: accrue-savings
slug: accrue-savings-domain-security
source_filename: accrue-savings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.byaccrue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:28:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.byaccrue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 02:43:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: merchant-api.accruesavings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: byaccrue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: accruesavings.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accrue-savings/refs/heads/main/security/accrue-savings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Loyalty
- Wallets
- Stored Value
- Rewards
- Banking
- Fintech
- Webhooks
---
