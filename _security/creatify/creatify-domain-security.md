---
api_specs:
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify AI Avatar API
  slug: creatify-ai-avatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Link-to-Video API
  slug: creatify-link-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify AI Shorts API
  slug: creatify-ai-shorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Custom Templates API
  slug: creatify-custom-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Product-to-Video API
  slug: creatify-product-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Text-to-Speech API
  slug: creatify-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Personas API
  slug: creatify-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Voices API
  slug: creatify-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Music API
  slug: creatify-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify AI Editing API
  slug: creatify-ai-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: creatify.ai
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:47086660.spf07.hubspotemail.net ~all
hosts:
- cert_expires: Oct  8 09:14:10 2026 GMT
  host: creatify.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: api.creatify.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
- cert_expires: Sep 11 02:07:26 2026 GMT
  host: docs.creatify.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
kind: domain-security
layout: security
method: probed
name: Creatify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creatify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS; 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Creatify
provider_slug: creatify
slug: creatify-domain-security
source_filename: creatify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creatify.ai\n  https: true\n  cert_expires: Oct  8 09:14:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.creatify.ai\n  https: true\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: docs.creatify.ai\n  https: true\n  cert_expires: Sep 11 02:07:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: creatify.ai\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:47086660.spf07.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/security/creatify-domain-security.yml
summary_line: HSTS · DMARC
tags:
- AI Avatars
- Video Generation
- AI Video
- Generative AI
- Marketing Video
- Text to Speech
- UGC Ads
- AI Avatar
---
