---
api_specs:
- filename: allmodels-account-api-openapi.yml
  format: yaml
  label: Allmodels Account API
  slug: allmodels-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-account-api-openapi.yml
- filename: allmodels-allmodels-api-api-openapi.yml
  format: yaml
  label: Allmodels Allmodels API
  slug: allmodels-allmodels-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-allmodels-api-api-openapi.yml
- filename: allmodels-custom-voices-api-openapi.yml
  format: yaml
  label: Allmodels Custom Voices API
  slug: allmodels-custom-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-custom-voices-api-openapi.yml
- filename: allmodels-el-api-openapi.yml
  format: yaml
  label: Allmodels El API
  slug: allmodels-el-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-el-api-openapi.yml
- filename: allmodels-health-api-openapi.yml
  format: yaml
  label: Allmodels Health API
  slug: allmodels-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-health-api-openapi.yml
- filename: allmodels-oai-api-openapi.yml
  format: yaml
  label: Allmodels Oai API
  slug: allmodels-oai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-oai-api-openapi.yml
- filename: allmodels-realtime-api-openapi.yml
  format: yaml
  label: Allmodels Realtime API
  slug: allmodels-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-realtime-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allmodels.io
  spf: true
hosts:
- cert_expires: Jan 10 08:14:59 2027 GMT
  host: allmodels.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Allmodels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allmodels, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allmodels
provider_slug: allmodels
slug: allmodels-domain-security
source_filename: allmodels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allmodels.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 08:14:59 2027 GMT\n  hsts: false\ndomains:\n- domain: allmodels.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/security/allmodels-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- VoiceAI
- TextToSpeech
- SpeechToText
- Real-Time
---
