---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yunjichina.com.cn
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: yunjichina.com.cn
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yunjichina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yunji, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yunji
provider_slug: yunjichina
slug: yunjichina-domain-security
source_filename: yunjichina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yunjichina.com.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: yunjichina.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yunjichina/refs/heads/main/security/yunjichina-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- E-Commerce
- Social Commerce
- Retail
- Marketplace
- China
- Consumer
---
