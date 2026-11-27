---
api_specs:
- filename: flowspeech-quota-api-openapi.yml
  format: yaml
  label: FlowSpeech Quota API
  slug: flowspeech-quota-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowspeech/openapi/flowspeech-quota-api-openapi.yml
- filename: flowspeech-tts-api-openapi.yml
  format: yaml
  label: FlowSpeech Tts API
  slug: flowspeech-tts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowspeech/openapi/flowspeech-tts-api-openapi.yml
- filename: flowspeech-voices-api-openapi.yml
  format: yaml
  label: FlowSpeech Voices API
  slug: flowspeech-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowspeech/openapi/flowspeech-voices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flowspeech.io
  spf: true
hosts:
- cert_expires: Jan  5 11:02:49 2027 GMT
  host: flowspeech.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FlowSpeech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlowSpeech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FlowSpeech
provider_slug: flowspeech
slug: flowspeech-domain-security
source_filename: flowspeech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowspeech.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 11:02:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flowspeech.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flowspeech/security/flowspeech-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Text-to-Speech
- Artificial Intelligence
- Voice
- Asynchronous
---
