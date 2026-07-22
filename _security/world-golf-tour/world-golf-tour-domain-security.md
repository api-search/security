---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wgt.com
  spf: true
hosts:
- cert_expires: Sep 25 11:29:29 2026 GMT
  host: www.wgt.com
  hsts: true
  hsts_max_age: 864000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: World Golf Tour Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Golf Tour, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: World Golf Tour
provider_slug: world-golf-tour
slug: world-golf-tour-domain-security
source_filename: world-golf-tour-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wgt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:29:29 2026 GMT\n  hsts: true\n  hsts_max_age: 864000\ndomains:\n- domain: wgt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world-golf-tour/refs/heads/main/security/world-golf-tour-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Golf
- Gaming
- Sports
- Simulation
- Entertainment
- Mobile
---
