---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carswitch.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: carswitch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carswitch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarSwitch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CarSwitch
provider_slug: carswitch
slug: carswitch-domain-security
source_filename: carswitch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carswitch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: carswitch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carswitch/refs/heads/main/security/carswitch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Used Cars
- Marketplace
- Automotive Marketplace
- E-Commerce
- Car Financing
- Vehicle Inspection
- United Arab Emirates
- Saudi Arabia
---
