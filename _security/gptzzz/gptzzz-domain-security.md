---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gptzzz.ai
  spf: true
hosts:
- cert_expires: Nov 26 20:51:15 2026 GMT
  host: gptzzz.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gptzzz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KaiGPT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KaiGPT
provider_slug: gptzzz
slug: gptzzz-domain-security
source_filename: gptzzz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gptzzz.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 20:51:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gptzzz.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gptzzz/refs/heads/main/security/gptzzz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM Gateway
- API Relay
- OpenAI-Compatible
- Claude
- Gemini
- LLM
- China
---
