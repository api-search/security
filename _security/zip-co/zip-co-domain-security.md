---
api_specs:
- filename: llms.txt
  format: yaml
  label: Zip Global Merchant API
  slug: zip-global-merchant-api
  spec_type: OpenAPI
  url: https://developers.zip.co/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zip.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: merchant-api.com
  spf: false
hosts:
- cert_expires: Oct  2 17:00:00 2026 GMT
  host: developers.zip.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 11:03:06 2026 GMT
  host: zip.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 22:59:47 2026 GMT
  host: sand.merchant-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zip Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zip, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zip
provider_slug: zip-co
slug: zip-co-domain-security
source_filename: zip-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.zip.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:00:00 2026 GMT\n  hsts: null\n- host: zip.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:03:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sand.merchant-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 22:59:47 2026 GMT\n  hsts: null\ndomains:\n- domain: zip.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: merchant-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zip-co/refs/heads/main/security/zip-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BNPL
- Buy Now Pay Later
- Digital Wallet
- Payments
- Fintech
- Checkout
- Merchant Services
---
