---
api_specs:
- filename: memories-platform-openapi.json
  format: json
  label: Memories.ai Platform API
  slug: memoriesai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memories/refs/heads/main/openapi/memories-platform-openapi.json
- filename: memories-stream-understanding-openapi.json
  format: json
  label: Memories.ai Stream Video Understanding API
  slug: memoriesai-stream-video-understanding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memories/refs/heads/main/openapi/memories-stream-understanding-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: memories.ai
  spf: true
hosts:
- cert_expires: Aug 24 06:54:49 2026 GMT
  host: memories.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 20:36:42 2026 GMT
  host: api-tools.memories.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 19:28:20 2026 GMT
  host: api.memories.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memories Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memories, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Memories
provider_slug: memories
slug: memories-domain-security
source_filename: memories-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memories.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:54:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-tools.memories.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:36:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.memories.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:28:20 2026 GMT\n  hsts: null\ndomains:\n- domain: memories.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memories/refs/heads/main/security/memories-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Video Intelligence
- Video Understanding
- Video Search
- Transcription
- Embeddings
- Multimodal AI
- Content Moderation
- AI Agents
- Machine Learning
---
