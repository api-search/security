---
api_specs:
- filename: llms.txt
  format: yaml
  label: Recall.ai REST API
  slug: recallai-rest-api
  spec_type: OpenAPI
  url: https://docs.recall.ai/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: recall.ai
  spf: true
hosts:
- cert_expires: Sep  1 10:47:17 2026 GMT
  host: www.recall.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 12:55:18 2026 GMT
  host: docs.recall.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: us-east-1.recall.ai
  hsts: true
  hsts_max_age: 60
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recall Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recall.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Recall.ai
provider_slug: recall-ai
slug: recall-ai-domain-security
source_filename: recall-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.recall.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 10:47:17 2026 GMT\n  hsts: false\n- host: docs.recall.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:55:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us-east-1.recall.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 60\ndomains:\n- domain: recall.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recall-ai/refs/heads/main/security/recall-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Meeting Bots
- Recording
- Transcription
- Video Conferencing
- Zoom
- Google Meet
- Microsoft Teams
- Real-Time
- AI
- Infrastructure
---
