---
api_specs:
- filename: llms.txt
  format: yaml
  label: Lemonway API
  slug: lemonway-api
  spec_type: OpenAPI
  url: https://documentation.lemonway.com/llms.txt
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lemonway.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.lemonway.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 07:36:31 2026 GMT
  host: documentation.lemonway.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.lemonway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemonway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemonway, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Lemonway
provider_slug: lemonway
slug: lemonway-domain-security
source_filename: lemonway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lemonway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.lemonway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:36:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lemonway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lemonway.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonway/refs/heads/main/security/lemonway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Marketplace
- IBAN
- KYC
- Wallets
- Bank Transfers
- Card Payments
- Crowdfunding
- European
- PSD2
---
