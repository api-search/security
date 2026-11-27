---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mylasertools.com
  spf: true
hosts:
- cert_expires: Feb 14 05:35:18 2027 GMT
  host: mylasertools.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MyLaserTools.com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyLaserTools.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyLaserTools.com
provider_slug: mylasertools-com
slug: mylasertools-com-domain-security
source_filename: mylasertools-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mylasertools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 05:35:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mylasertools.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mylasertools-com/security/mylasertools-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Laser Cutting
- CNC Machining
- 3D Printing
- Design Generators
- Maker Tools
---
