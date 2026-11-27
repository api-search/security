---
api_specs:
- filename: justtranscribe-ai-me-api-openapi.yml
  format: yaml
  label: JustTranscribe Me API
  slug: justtranscribe-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justtranscribe-ai/openapi/justtranscribe-ai-me-api-openapi.yml
- filename: justtranscribe-ai-transcripts-api-openapi.yml
  format: yaml
  label: JustTranscribe Transcripts API
  slug: justtranscribe-ai-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justtranscribe-ai/openapi/justtranscribe-ai-transcripts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: justtranscribe.ai
  spf: true
hosts:
- cert_expires: Jan  2 23:37:25 2027 GMT
  host: justtranscribe.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JustTranscribe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JustTranscribe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JustTranscribe
provider_slug: justtranscribe-ai
slug: justtranscribe-ai-domain-security
source_filename: justtranscribe-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justtranscribe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:37:25 2027 GMT\n  hsts: false\ndomains:\n- domain: justtranscribe.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/justtranscribe-ai/security/justtranscribe-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transcription
- Audio
- Video
- Artificial Intelligence
- Free
- Software-as-a-Service
---
