---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hyde.ai
  spf: false
hosts:
- cert_expires: Aug 27 13:38:08 2026 GMT
  host: hyde.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyde Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyde, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Hyde
provider_slug: hyde
slug: hyde-domain-security
source_filename: hyde-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyde.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hyde.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyde/refs/heads/main/security/hyde-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Artificial Intelligence
- Machine Learning
- Reasoning Models
- Enterprise AI
- Model Training
- LLM
---
