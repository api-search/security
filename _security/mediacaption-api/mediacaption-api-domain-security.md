---
api_specs:
- filename: mediacaption-api-balance-api-openapi.yml
  format: yaml
  label: MediaCaption API Balance API
  slug: mediacaption-api-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediacaption-api/openapi/mediacaption-api-balance-api-openapi.yml
- filename: mediacaption-api-jobs-api-openapi.yml
  format: yaml
  label: MediaCaption API Jobs API
  slug: mediacaption-api-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediacaption-api/openapi/mediacaption-api-jobs-api-openapi.yml
- filename: mediacaption-api-transcriptions-api-openapi.yml
  format: yaml
  label: MediaCaption API Transcriptions API
  slug: mediacaption-api-transcriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediacaption-api/openapi/mediacaption-api-transcriptions-api-openapi.yml
- filename: mediacaption-api-transcripts-api-openapi.yml
  format: yaml
  label: MediaCaption API Transcripts API
  slug: mediacaption-api-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediacaption-api/openapi/mediacaption-api-transcripts-api-openapi.yml
- filename: mediacaption-api-uploads-api-openapi.yml
  format: yaml
  label: MediaCaption API Uploads API
  slug: mediacaption-api-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediacaption-api/openapi/mediacaption-api-uploads-api-openapi.yml
- filename: mediacaption-api-user-api-openapi.yml
  format: yaml
  label: MediaCaption API User API
  slug: mediacaption-api-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediacaption-api/openapi/mediacaption-api-user-api-openapi.yml
- filename: mediacaption-api-webhooks-api-openapi.yml
  format: yaml
  label: MediaCaption API Webhooks API
  slug: mediacaption-api-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediacaption-api/openapi/mediacaption-api-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mediacaption.io
  spf: false
hosts:
- cert_expires: Dec  7 10:10:55 2026 GMT
  host: mediacaption.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 12:30:03 2027 GMT
  host: www.mediacaption.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 10:37:43 2026 GMT
  host: api.mediacaption.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: MediaCaption API Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediaCaption API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: MediaCaption API
provider_slug: mediacaption-api
slug: mediacaption-api-domain-security
source_filename: mediacaption-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mediacaption.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 10:10:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.mediacaption.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 12:30:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mediacaption.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 10:37:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mediacaption.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mediacaption-api/security/mediacaption-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- YouTube
- Transcription
- Captions
- Subtitles
- Video
- REST
- OpenAPI
- Webhook
- Speech-to-Text
- Media
- Developer Tools
---
