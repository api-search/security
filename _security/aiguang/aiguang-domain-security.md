---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: guang.com
  spf: true
hosts:
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: www.guang.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiguang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aiguang, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aiguang
provider_slug: aiguang
slug: aiguang-domain-security
source_filename: aiguang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guang.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: guang.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiguang/refs/heads/main/security/aiguang-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Live Commerce
- Live Streaming
- Social Commerce
- Retail
- Video
- WeChat
- China
- Marketplace
---
