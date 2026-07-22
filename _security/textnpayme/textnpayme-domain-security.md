---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: textnpayme.com
  spf: true
hosts:
- cert_expires: Mar 29 23:59:59 2027 GMT
  host: textnpayme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Textnpayme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Text''nPayMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Text'nPayMe
provider_slug: textnpayme
slug: textnpayme-domain-security
source_filename: textnpayme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: textnpayme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: textnpayme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textnpayme/refs/heads/main/security/textnpayme-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Fintech
- Embedded Payments
- Payment Gateway
- SDK
- Mobile Payments
- Banking
- Cross-Border Payments
---
