---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buyersense.ai
  spf: true
hosts:
- cert_expires: Jan 14 17:14:01 2027 GMT
  host: buyersense.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BuyerSense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuyerSense, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BuyerSense
provider_slug: buyersense-ai
slug: buyersense-ai-domain-security
source_filename: buyersense-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buyersense.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 17:14:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buyersense.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buyersense-ai/security/buyersense-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- B2B
- Software-as-a-Service
- Optimization
- AgentReasoning
---
