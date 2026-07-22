---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: isidor.ai
  spf: true
hosts:
- cert_expires: Oct 16 19:38:08 2026 GMT
  host: isidor.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Isidor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Isidor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Isidor
provider_slug: isidor
slug: isidor-domain-security
source_filename: isidor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isidor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: isidor.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isidor/refs/heads/main/security/isidor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Enterprise AI
- Machine Learning
- Data Pipelines
- Model Training
- Evaluation
- LLM
---
