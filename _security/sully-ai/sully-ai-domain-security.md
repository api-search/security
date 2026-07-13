---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sully.ai
  spf: true
hosts:
- cert_expires: Aug 15 23:59:59 2026 GMT
  host: www.sully.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 15:16:41 2026 GMT
  host: docs.sully.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 17:59:43 2026 GMT
  host: api.sully.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sully Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sully AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Sully AI
provider_slug: sully-ai
slug: sully-ai-domain-security
source_filename: sully-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sully.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sully.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:16:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sully.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:59:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sully.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sully-ai/refs/heads/main/security/sully-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Health Tech
- Medical AI
- Clinical AI
- AI Scribe
- Ambient Scribe
- Clinical Documentation
- SOAP Notes
- Medical Coding
- ICD-10
- CPT
- SNOMED
- Speech to Text
- Audio Transcription
- Real Time Streaming
- WebSockets
- Webhooks
- EHR Integration
- Epic
- Cerner
- HIPAA
- AI Agents
- Workflow Automation
- Healthcare Automation
---
