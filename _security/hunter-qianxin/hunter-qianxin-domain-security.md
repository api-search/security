---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qianxin.com
  spf: true
hosts:
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: hunter.qianxin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hunter (Qi An Xin) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hunter (Qi An Xin), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hunter (Qi An Xin)
provider_slug: hunter-qianxin
slug: hunter-qianxin-domain-security
source_filename: hunter-qianxin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hunter.qianxin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: qianxin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hunter-qianxin/security/hunter-qianxin-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
