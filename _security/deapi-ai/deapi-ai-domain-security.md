---
api_specs:
- filename: deapi-ai-client-api-api-openapi.yml
  format: yaml
  label: deapi-ai Client API
  slug: deapi-ai-client-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deapi-ai/openapi/deapi-ai-client-api-api-openapi.yml
- filename: deapi-ai-client-api-v2-api-openapi.yml
  format: yaml
  label: deapi-ai Client API v2 API
  slug: deapi-ai-client-api-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deapi-ai/openapi/deapi-ai-client-api-v2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deapi.ai
  spf: true
hosts:
- cert_expires: Jan 23 12:56:25 2027 GMT
  host: deapi.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deapi Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for deapi-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: deapi-ai
provider_slug: deapi-ai
slug: deapi-ai-domain-security
source_filename: deapi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 12:56:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deapi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/deapi-ai/security/deapi-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Generative AI
- API
- Open-source
- Image Generation
- Text-to-Speech
- Video Transcription
---
