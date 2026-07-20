---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: baidu.com
  spf: true
hosts:
- cert_expires: Aug 10 07:01:01 2026 GMT
  host: www.baidu.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Baidu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baidu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Baidu
provider_slug: baidu
slug: baidu-domain-security
source_filename: baidu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baidu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 07:01:01 2026 GMT\n  hsts: false\ndomains:\n- domain: baidu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baidu/refs/heads/main/security/baidu-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Technology
- Artificial Intelligence
- Machine Learning
- LLM
- Maps
- Geolocation
- Cloud
- China
---
