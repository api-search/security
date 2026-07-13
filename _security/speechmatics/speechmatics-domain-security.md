---
api_specs:
- filename: batch.yaml
  format: yaml
  label: Speechmatics Batch Transcription API
  slug: batch-transcription-api
  spec_type: OpenAPI
  url: https://docs.speechmatics.com/batch.yaml
- filename: speechmatics-management-api-openapi.yml
  format: yaml
  label: Speechmatics Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechmatics/refs/heads/main/openapi/speechmatics-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: speechmatics.com
  spf: true
hosts:
- cert_expires: Sep 15 16:59:13 2026 GMT
  host: www.speechmatics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 02:18:41 2026 GMT
  host: portal.speechmatics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 22:12:07 2026 GMT
  host: docs.speechmatics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speechmatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Speechmatics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Speechmatics
provider_slug: speechmatics
slug: speechmatics-domain-security
source_filename: speechmatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.speechmatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:59:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.speechmatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.speechmatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:12:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: speechmatics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speechmatics/refs/heads/main/security/speechmatics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Speech Recognition
- Speech-to-Text
- Transcription
- Real-Time Transcription
- Batch Transcription
- Speaker Diarization
- Text-to-Speech
- Voice AI
- NLP
- Audio Processing
- WebSocket
- REST
---
