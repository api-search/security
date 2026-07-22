---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: withmartian.com
  spf: true
hosts:
- cert_expires: Aug 31 07:54:02 2026 GMT
  host: withmartian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 00:31:05 2026 GMT
  host: docs.withmartian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:12:32 2026 GMT
  host: api.withmartian.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Martian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Martian, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Martian
provider_slug: martian
slug: martian-domain-security
source_filename: martian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withmartian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:54:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.withmartian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:31:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.withmartian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:12:32 2026 GMT\n  hsts: null\ndomains:\n- domain: withmartian.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/martian/refs/heads/main/security/martian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- LLM Gateway
- Model Router
- Machine Learning
- Interpretability
- Inference
- OpenAI Compatible
- Developer Tools
---
