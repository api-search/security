---
api_specs:
- filename: nala-rafiki-openapi.yml
  format: yaml
  label: Rafiki API
  slug: rafiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nala/refs/heads/main/openapi/nala-rafiki-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nala.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rafiki.com
  spf: true
hosts:
- cert_expires: Aug 24 06:58:53 2026 GMT
  host: www.nala.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 16:58:45 2026 GMT
  host: docs.rafiki.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: rest.prod.rafiki-api.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NALA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NALA
provider_slug: nala
slug: nala-domain-security
source_filename: nala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:58:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.rafiki.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 16:58:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.prod.rafiki-api.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nala.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rafiki.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nala/refs/heads/main/security/nala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Remittances
- Money Transfer
- Payouts
- Cross-Border Payments
- Mobile Money
- Stablecoins
- Africa
---
