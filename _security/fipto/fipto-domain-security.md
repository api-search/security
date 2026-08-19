---
api_specs:
- filename: fipto-customer-api-openapi.yml
  format: yaml
  label: Fipto API
  slug: customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-customer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fipto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fipto.app
  spf: true
hosts:
- cert_expires: Nov  9 04:52:31 2026 GMT
  host: fipto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 13:06:19 2026 GMT
  host: docs.fipto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: api.fipto.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fipto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fipto, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fipto
provider_slug: fipto
slug: fipto-domain-security
source_filename: fipto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fipto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 04:52:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fipto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 13:06:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fipto.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: fipto.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fipto.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/security/fipto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Payments
- Stablecoins
- Banking
- Treasury
- Cross-Border Payments
- Digital Currency
- Fintech
- Wallets
---
