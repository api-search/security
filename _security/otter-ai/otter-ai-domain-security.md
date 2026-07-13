---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: otter.ai
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: otter.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.otter.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Otter Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otter.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Otter.ai
provider_slug: otter-ai
slug: otter-ai-domain-security
source_filename: otter-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otter.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\n- host: api.otter.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: otter.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otter-ai/refs/heads/main/security/otter-ai-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- AI
- Transcription
- Meeting Notes
- Speech-to-Text
- Speaker Identification
- Meeting Intelligence
- Summaries
---
