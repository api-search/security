---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getmaxim.ai
  spf: true
hosts:
- cert_expires: Sep  9 12:04:49 2026 GMT
  host: www.getmaxim.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 12:40:07 2026 GMT
  host: api.getmaxim.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maxim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maxim AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Maxim AI
provider_slug: maxim
slug: maxim-domain-security
source_filename: maxim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getmaxim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 12:04:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getmaxim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:40:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getmaxim.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxim/refs/heads/main/security/maxim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- LLM
- Agents
- Observability
- Evaluation
- Simulation
- Tracing
- Prompts
- Datasets
- Monitoring
- Voice
- OpenTelemetry
---
