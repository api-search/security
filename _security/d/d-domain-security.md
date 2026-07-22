---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: d.cn
  spf: false
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: d.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Downjoy (当乐网), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Downjoy (当乐网)
provider_slug: d
slug: d-domain-security
source_filename: d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: d.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: d.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d/refs/heads/main/security/d-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Mobile Games
- Gaming
- Game Distribution
- Developer Platform
- SDK
- China
---
