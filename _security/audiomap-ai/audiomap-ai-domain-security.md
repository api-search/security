---
api_specs:
- filename: audiomap-ai-ask-api-openapi.yml
  format: yaml
  label: AudioMap Ask API
  slug: audiomap-ai-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audiomap-ai/openapi/audiomap-ai-ask-api-openapi.yml
- filename: audiomap-ai-content-api-openapi.yml
  format: yaml
  label: AudioMap Content API
  slug: audiomap-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audiomap-ai/openapi/audiomap-ai-content-api-openapi.yml
- filename: audiomap-ai-deliverables-api-openapi.yml
  format: yaml
  label: AudioMap Deliverables API
  slug: audiomap-ai-deliverables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audiomap-ai/openapi/audiomap-ai-deliverables-api-openapi.yml
- filename: audiomap-ai-notes-api-openapi.yml
  format: yaml
  label: AudioMap Notes API
  slug: audiomap-ai-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audiomap-ai/openapi/audiomap-ai-notes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: audiomap.ai
  spf: true
hosts:
- cert_expires: Jan 23 22:20:13 2027 GMT
  host: audiomap.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AudioMap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AudioMap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AudioMap
provider_slug: audiomap-ai
slug: audiomap-ai-domain-security
source_filename: audiomap-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audiomap.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 22:20:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: audiomap.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/audiomap-ai/security/audiomap-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Transcription
- Audio
- Meeting Notes
- Europe
---
