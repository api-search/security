---
api_specs:
- filename: assemblyai-openapi-original.yml
  format: yaml
  label: AssemblyAI API
  slug: assemblyai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assemblyai/refs/heads/main/openapi/assemblyai-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: assemblyai.com
  spf: true
hosts:
- cert_expires: Aug 28 06:20:42 2026 GMT
  host: www.assemblyai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.assemblyai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Assemblyai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AssemblyAI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AssemblyAI
provider_slug: assemblyai
slug: assemblyai-domain-security
source_filename: assemblyai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.assemblyai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 06:20:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.assemblyai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: assemblyai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assemblyai/refs/heads/main/security/assemblyai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Audio
- Speech
- Transcription
- Speech to Text
---
