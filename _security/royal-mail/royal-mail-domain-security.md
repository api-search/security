---
api_specs:
- filename: click-and-drop-api-v1.yaml
  format: yaml
  label: Royal Mail Click & Drop API
  slug: royal-mail-click-drop-api
  spec_type: OpenAPI
  url: https://api.parcel.royalmail.com/doc/v1/click-and-drop-api-v1.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: royalmail.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: royalmail.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: developer.royalmail.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.royalmail.net
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 20 23:44:09 2026 GMT
  host: help.parcel.royalmail.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Royal Mail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Royal Mail, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Royal Mail
provider_slug: royal-mail
slug: royal-mail-domain-security
source_filename: royal-mail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.royalmail.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.royalmail.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\n- host: help.parcel.royalmail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:44:09 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: royalmail.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: royalmail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/royal-mail/refs/heads/main/security/royal-mail-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Shipping
- Postal Services
- Labels
- Tracking
- Logistics
- Barcodes
- Click and Drop
- UK
---
