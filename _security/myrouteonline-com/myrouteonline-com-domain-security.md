---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myrouteonline.com
  spf: true
hosts:
- cert_expires: Jan 13 21:48:35 2027 GMT
  host: myrouteonline.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MyRouteOnline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyRouteOnline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyRouteOnline
provider_slug: myrouteonline-com
slug: myrouteonline-com-domain-security
source_filename: myrouteonline-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myrouteonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 21:48:35 2027 GMT\n  hsts: false\ndomains:\n- domain: myrouteonline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/myrouteonline-com/security/myrouteonline-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Route Planning
- Logistics
- Fleet Management
- Delivery Software
- Multi‑Stop Routing
- GPS Navigation
---
