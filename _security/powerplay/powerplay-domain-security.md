---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getpowerplay.in
  spf: false
hosts:
- cert_expires: Sep 23 06:52:52 2026 GMT
  host: www.getpowerplay.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powerplay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Powerplay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Powerplay
provider_slug: powerplay
slug: powerplay-domain-security
source_filename: powerplay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getpowerplay.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:52:52 2026 GMT\n  hsts: false\ndomains:\n- domain: getpowerplay.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerplay/refs/heads/main/security/powerplay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud Saas
- Construction
- Construction Technology
- Project Management
- Field Service
- Payroll
- Mobile Apps
---
