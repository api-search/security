---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gowabi.com
  spf: true
hosts:
- cert_expires: Sep 18 04:52:54 2026 GMT
  host: gowabi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gowabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoWabi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GoWabi
provider_slug: gowabi
slug: gowabi-domain-security
source_filename: gowabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gowabi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:52:54 2026 GMT\n  hsts: false\ndomains:\n- domain: gowabi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gowabi/refs/heads/main/security/gowabi-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Beauty
- Wellness
- Booking
- Marketplace
- Spa
- Consumer
- Southeast Asia
- Thailand
---
