---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coohua.com
  spf: false
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.coohua.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Coohua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for coohua, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: coohua
provider_slug: coohua
slug: coohua-domain-security
source_filename: coohua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coohua.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: coohua.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coohua/refs/heads/main/security/coohua-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Advertising
- Mobile
- AdTech
- Incentive Advertising
- China
- Consumer
---
