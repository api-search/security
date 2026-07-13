---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: whu.edu.cn
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: en.whu.edu.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wuhan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wuhan University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Wuhan University
provider_slug: wuhan
slug: wuhan-domain-security
source_filename: wuhan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.whu.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whu.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wuhan/refs/heads/main/security/wuhan-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Education
- Higher Education
- University
- Research
- China
- Open Source
---
