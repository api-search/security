---
api_specs:
- filename: transcriptapi-io-openapi.json
  format: json
  label: TranscriptAPI
  slug: transcriptapi
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-io/openapi/transcriptapi-io-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: transcriptapi.io
  spf: true
hosts:
- cert_expires: Dec  5 17:05:25 2026 GMT
  host: transcriptapi.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Transcriptapi Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for transcriptapi-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: transcriptapi-io
provider_slug: transcriptapi-io
slug: transcriptapi-io-domain-security
source_filename: transcriptapi-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transcriptapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 17:05:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: transcriptapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/transcriptapi-io/security/transcriptapi-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- YouTube
- Transcripts
- API
- Video
- Data
---
