---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: one1.cn
  spf: false
hosts:
- cert_expires: Dec 20 23:27:39 2026 GMT
  host: one1.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: one1-cn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for one1-cn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: one1-cn
provider_slug: one1-cn
slug: one1-cn-domain-security
source_filename: one1-cn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: one1.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:27:39 2026 GMT\n  hsts: false\ndomains:\n- domain: one1.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/one1-cn/security/one1-cn-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Trademarks
- Risk Detection
- E-Commerce
- China
---
