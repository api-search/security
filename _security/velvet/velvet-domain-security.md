---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: velvetlab.ai
  spf: false
hosts:
- cert_expires: Aug 24 18:40:28 2026 GMT
  host: velvetlab.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Velvet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velvet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Velvet
provider_slug: velvet
slug: velvet-domain-security
source_filename: velvet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: velvetlab.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:40:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: velvetlab.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velvet/refs/heads/main/security/velvet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Multimodal AI
- Machine Learning
- Datasets
- Model Evaluation
- Video
- World Models
- Y Combinator
---
