---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thinkingmachines.ai
  spf: true
hosts:
- cert_expires: Oct  1 08:32:28 2026 GMT
  host: thinkingmachines.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 28 22:02:34 2026 GMT
  host: tinker-docs.thinkingmachines.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  3 11:19:57 2026 GMT
  host: tinker.thinkingmachines.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Thinking Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thinking Machines, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Thinking Machines
provider_slug: thinking-machines
slug: thinking-machines-domain-security
source_filename: thinking-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thinkingmachines.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 08:32:28 2026 GMT\n  hsts: false\n- host: tinker-docs.thinkingmachines.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 28 22:02:34 2026 GMT\n  hsts: false\n- host: tinker.thinkingmachines.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 11:19:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thinkingmachines.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thinking-machines/refs/heads/main/security/thinking-machines-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Machine Learning
- Fine-Tuning
- LLM
- Model Training
- Developer Tools
---
