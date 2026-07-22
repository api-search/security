---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: withdavid.ai
  spf: true
hosts:
- cert_expires: Jan 28 17:27:14 2027 GMT
  host: withdavid.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: David Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for David AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: David AI
provider_slug: david-ai
slug: david-ai-domain-security
source_filename: david-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withdavid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 17:27:14 2027 GMT\n  hsts: null\ndomains:\n- domain: withdavid.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/david-ai/refs/heads/main/security/david-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Machine Learning
- Audio Data
- Speech Recognition
- Conversational AI
- Voice
- Datasets
---
