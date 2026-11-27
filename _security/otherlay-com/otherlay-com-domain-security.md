---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: otherlay.com
  spf: true
hosts:
- cert_expires: Jan 25 15:44:10 2027 GMT
  host: otherlay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Otherlay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otherlay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Otherlay
provider_slug: otherlay-com
slug: otherlay-com-domain-security
source_filename: otherlay-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otherlay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 25 15:44:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: otherlay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/otherlay-com/security/otherlay-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Apple Silicon
- Mac Rental
- Cloud Development
- Remote Desktop
- Developer Tools
---
