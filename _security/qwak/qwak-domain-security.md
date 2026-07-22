---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qwak.com
  spf: true
hosts:
- cert_expires: Sep 11 16:49:03 2026 GMT
  host: www.qwak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qwak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qwak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qwak
provider_slug: qwak
slug: qwak-domain-security
source_filename: qwak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qwak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:49:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qwak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwak/refs/heads/main/security/qwak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Machine Learning
- MLOps
- LLMOps
- Feature Store
- Model Deployment
- Model Monitoring
- Developer Tools
---
