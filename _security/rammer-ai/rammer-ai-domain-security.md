---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: rammer.ai
  spf: true
hosts:
- cert_expires: Dec 22 05:37:36 2026 GMT
  host: rammer.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rammer Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symbl.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Symbl.ai
provider_slug: rammer-ai
slug: rammer-ai-domain-security
source_filename: rammer-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rammer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 05:37:36 2026 GMT\n  hsts: null\ndomains:\n- domain: rammer.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://artifacts.apis.io/rammer-ai/security/rammer-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Conversation
- Speech
- NLP
- Real-time
- Communication
---
