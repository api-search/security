---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: transwarp.cn
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.transwarp.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transwarp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transwarp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Transwarp
provider_slug: transwarp
slug: transwarp-domain-security
source_filename: transwarp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transwarp.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: transwarp.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transwarp/refs/heads/main/security/transwarp-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Big Data
- Databases
- Vector Databases
- Artificial Intelligence
- Data Analytics
- Graph Databases
- China
---
