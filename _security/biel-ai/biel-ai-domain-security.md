---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biel.ai
  spf: true
hosts:
- cert_expires: Dec 19 01:38:09 2026 GMT
  host: biel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biel Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for biel-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: biel-ai
provider_slug: biel-ai
slug: biel-ai-domain-security
source_filename: biel-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 01:38:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: biel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/biel-ai/security/biel-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Documentation
- Assistant
- Retrieval-Augmented Generation
- Integration
---
