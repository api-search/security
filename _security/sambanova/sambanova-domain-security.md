---
api_specs:
- filename: sambanova-openapi.yml
  format: yaml
  label: SambaCloud API
  slug: sambacloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova/refs/heads/main/openapi/sambanova-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sambanova.ai
  spf: true
hosts:
- cert_expires: Aug 13 18:56:43 2026 GMT
  host: sambanova.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:04:00 2027 GMT
  host: docs.sambanova.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:04:00 2027 GMT
  host: api.sambanova.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sambanova Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SambaNova, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SambaNova
provider_slug: sambanova
slug: sambanova-domain-security
source_filename: sambanova-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sambanova.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 18:56:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sambanova.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:04:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sambanova.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:04:00 2027 GMT\n  hsts: null\ndomains:\n- domain: sambanova.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sambanova/refs/heads/main/security/sambanova-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Inference
- Large Language Models
- Dataflow
- Hardware
- Cloud
- OpenAI Compatible
- Sovereign AI
- SDK
- Accelerator
- Open Source
---
