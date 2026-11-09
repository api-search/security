---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ai-rook.com
  spf: false
hosts:
- cert_expires: Jan 24 05:36:53 2027 GMT
  host: ai-rook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ai Rook Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Rook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: AI Rook
provider_slug: ai-rook-com
slug: ai-rook-com-domain-security
source_filename: ai-rook-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-rook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 05:36:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ai-rook.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ai-rook-com/security/ai-rook-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Autonomous
- Cryptocurrency
- LLM
- Payments
- Trading
---
