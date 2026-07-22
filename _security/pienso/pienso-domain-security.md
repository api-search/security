---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pienso.com
  spf: true
hosts:
- cert_expires: Oct  7 17:04:50 2026 GMT
  host: www.pienso.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pienso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pienso, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pienso
provider_slug: pienso
slug: pienso-domain-security
source_filename: pienso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pienso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:04:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pienso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pienso/refs/heads/main/security/pienso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Deep Learning
- Large Language Models
- Natural Language Processing
- No-Code
- Document Intelligence
- Data Analytics
---
