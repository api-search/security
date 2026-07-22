---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pokelabo.co.jp
  spf: true
hosts:
- cert_expires: Aug 28 07:24:13 2026 GMT
  host: pokelabo.co.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pokelabo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pokelabo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pokelabo
provider_slug: pokelabo
slug: pokelabo-domain-security
source_filename: pokelabo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pokelabo.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 07:24:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pokelabo.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pokelabo/refs/heads/main/security/pokelabo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Gaming
- Mobile Games
- Video Games
- Entertainment
- Japan
---
