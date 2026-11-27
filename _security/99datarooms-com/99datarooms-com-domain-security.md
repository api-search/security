---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: 99datarooms.com
  spf: true
hosts:
- cert_expires: Jan 11 21:22:19 2027 GMT
  host: 99datarooms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 99 Data Rooms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 99 Data Rooms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: 99 Data Rooms
provider_slug: 99datarooms-com
slug: 99datarooms-com-domain-security
source_filename: 99datarooms-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 99datarooms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 21:22:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 99datarooms.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/99datarooms-com/security/99datarooms-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Virtual Data Room
- Secure Sharing
- E-Signature
- UK-hosted
- GDPR
---
