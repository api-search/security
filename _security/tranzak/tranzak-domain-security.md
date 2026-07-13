---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tranzak.net
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tranzak.me
  spf: true
hosts:
- cert_expires: Sep  2 00:17:11 2026 GMT
  host: tranzak.net
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 11 01:09:35 2026 GMT
  host: docs.developer.tranzak.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 00:17:11 2026 GMT
  host: dsapi.tranzak.me
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tranzak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TranZak, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TranZak
provider_slug: tranzak
slug: tranzak-domain-security
source_filename: tranzak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tranzak.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  2 00:17:11 2026 GMT\n  hsts: false\n- host: docs.developer.tranzak.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 01:09:35 2026 GMT\n  hsts: false\n- host: dsapi.tranzak.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  2 00:17:11 2026 GMT\n  hsts: null\ndomains:\n- domain: tranzak.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: tranzak.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tranzak/refs/heads/main/security/tranzak-domain-security.yml
summary_line: TLSv1.2
tags:
- Fintech
- Mobile Money
- Payments
- Africa
- Cameroon
- Disbursements
- SMS
- Bill Payments
---
