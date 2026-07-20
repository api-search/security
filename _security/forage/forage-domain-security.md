---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinforage.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinforage.app
  spf: false
hosts:
- cert_expires: Sep 22 14:32:05 2026 GMT
  host: www.joinforage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 16:38:18 2026 GMT
  host: docs.joinforage.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.joinforage.app
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Forage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Forage
provider_slug: forage
slug: forage-domain-security
source_filename: forage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinforage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:32:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.joinforage.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 16:38:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.joinforage.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: joinforage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: joinforage.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/security/forage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- EBT
- SNAP
- EBT Cash
- HSA/FSA
- Fintech
- Government Benefits
- Grocery
- Checkout
- Financial Services
---
