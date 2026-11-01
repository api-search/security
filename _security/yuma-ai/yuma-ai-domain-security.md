---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yuma.ai
  spf: true
hosts:
- cert_expires: Dec 19 02:56:54 2026 GMT
  host: yuma.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yuma Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yuma AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yuma AI
provider_slug: yuma-ai
slug: yuma-ai-domain-security
source_filename: yuma-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yuma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 02:56:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: yuma.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/yuma-ai/security/yuma-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Machine-Learning
- Automation
- Data-Analysis
---
