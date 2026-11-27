---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: visionmenu.com
  spf: true
hosts:
- cert_expires: Feb 24 18:20:17 2027 GMT
  host: visionmenu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vision Menu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vision Menu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vision Menu
provider_slug: vision-menu
slug: vision-menu-domain-security
source_filename: vision-menu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: visionmenu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 18:20:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: visionmenu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/vision-menu/security/vision-menu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Dealership
- DigitalMenu
- Artificial Intelligence
---
