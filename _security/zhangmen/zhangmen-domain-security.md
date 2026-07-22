---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zhangmen.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.zhangmen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zhangmen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zhangmen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Zhangmen
provider_slug: zhangmen
slug: zhangmen-domain-security
source_filename: zhangmen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zhangmen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zhangmen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zhangmen/refs/heads/main/security/zhangmen-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Edtech
- Education
- Online Tutoring
- K-12
- E-Learning
- China
- Consumer
---
