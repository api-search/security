---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appboard.pro
  spf: true
hosts:
- cert_expires: Jan  5 14:57:59 2027 GMT
  host: appboard.pro
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appboard Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppBoard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AppBoard
provider_slug: appboard-pro
slug: appboard-pro-domain-security
source_filename: appboard-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appboard.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 14:57:59 2027 GMT\n  hsts: false\ndomains:\n- domain: appboard.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/appboard-pro/security/appboard-pro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Product Discovery
- Free
- Community
---
