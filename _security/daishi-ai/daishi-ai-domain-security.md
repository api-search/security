---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daishi.ai
  spf: true
hosts:
- cert_expires: Jan  5 09:49:09 2027 GMT
  host: daishi.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Daishi Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for daishi-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: daishi-ai
provider_slug: daishi-ai
slug: daishi-ai-domain-security
source_filename: daishi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daishi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 09:49:09 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: daishi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/daishi-ai/security/daishi-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Agents
- Platform
- Evaluation
- Simulation
- Marketplace
- Benchmark
---
