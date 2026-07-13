---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: suredbits.com
  spf: false
hosts:
- cert_expires: Aug 30 15:41:22 2026 GMT
  host: suredbits.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suredbits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuredBits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SuredBits
provider_slug: suredbits
slug: suredbits-domain-security
source_filename: suredbits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suredbits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:41:22 2026 GMT\n  hsts: null\ndomains:\n- domain: suredbits.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suredbits/refs/heads/main/security/suredbits-domain-security.yml
summary_line: TLSv1.3
tags:
- Sports And Fitness
- Public APIs
---
