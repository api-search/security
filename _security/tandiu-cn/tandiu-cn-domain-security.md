---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tandiu.cn
  spf: true
hosts:
- cert_expires: Jan 24 08:49:28 2027 GMT
  host: tandiu.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TANDIU Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TANDIU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TANDIU
provider_slug: tandiu-cn
slug: tandiu-cn-domain-security
source_filename: tandiu-cn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tandiu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 08:49:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tandiu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tandiu-cn/security/tandiu-cn-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Infrastructure
- Pricing
- Data
---
