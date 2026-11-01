---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: promptwave.ai
  spf: true
hosts:
- cert_expires: Nov  9 20:03:03 2026 GMT
  host: promptwave.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PromptWave AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PromptWave AI
provider_slug: promptwave
slug: promptwave-domain-security
source_filename: promptwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptwave.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 20:03:03 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: promptwave.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/promptwave/security/promptwave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Prompt Engineering
- Community
- Productivity
---
