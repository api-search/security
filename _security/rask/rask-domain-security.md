---
api_specs:
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Projects & Dubbing Jobs API
  slug: projects-dubbing-jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Translation API
  slug: translation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Transcription API
  slug: transcription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
- filename: rask-openapi.yml
  format: yaml
  label: Rask AI Job Status API
  slug: job-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/openapi/rask-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rask.ai
  spf: true
hosts:
- cert_expires: Aug 26 07:52:57 2026 GMT
  host: www.rask.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 06:25:04 2026 GMT
  host: docs.api.rask.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.rask.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rask Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rask AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rask AI
provider_slug: rask
slug: rask-domain-security
source_filename: rask-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rask.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:52:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.rask.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:25:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.rask.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rask.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rask/refs/heads/main/security/rask-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Video Localization
- Dubbing
- Translation
- Transcription
---
