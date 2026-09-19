---
api_specs:
- filename: transcriptfetch-system-api-openapi.yml
  format: yaml
  label: TranscriptFetch System API
  slug: transcriptfetch-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcriptfetch/refs/heads/main/openapi/transcriptfetch-system-api-openapi.yml
- filename: transcriptfetch-transcripts-api-openapi.yml
  format: yaml
  label: TranscriptFetch Transcripts API
  slug: transcriptfetch-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcriptfetch/refs/heads/main/openapi/transcriptfetch-transcripts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transcriptfetch.com
  spf: true
hosts:
- cert_expires: Nov  1 19:11:37 2026 GMT
  host: transcriptfetch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Transcriptfetch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TranscriptFetch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TranscriptFetch
provider_slug: transcriptfetch
slug: transcriptfetch-domain-security
source_filename: transcriptfetch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transcriptfetch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 19:11:37 2026 GMT\n  hsts: false\ndomains:\n- domain: transcriptfetch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcriptfetch/refs/heads/main/security/transcriptfetch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transcripts
- Speech-to-Text
- Captions
- YouTube
- TikTok
- Instagram
- Podcasts
- MCP
- llms-txt
- OpenAPI
- Transcription
- Video
- AI/LLM
- RAG
- Agents
- Developer Tools
- Media
- Content
- Spotify
- Apple Podcasts
---
