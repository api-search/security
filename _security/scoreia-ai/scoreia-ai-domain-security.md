---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scoreia.ai
  spf: false
hosts:
- cert_expires: Jan 27 11:27:42 2027 GMT
  host: scoreia.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scoreia Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for scoreia-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: scoreia-ai
provider_slug: scoreia-ai
slug: scoreia-ai-domain-security
source_filename: scoreia-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scoreia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 11:27:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scoreia.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/scoreia-ai/security/scoreia-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Benchmark
- MCP
- Gaming
---
