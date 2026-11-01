---
api_specs:
- filename: imgapi-ai-openapi-generated.yml
  format: yaml
  label: ImgAPI API
  slug: imgapi-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imgapi-ai/openapi/_ae-authored/imgapi-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imgapi.ai
  spf: true
hosts:
- cert_expires: Jan  4 14:04:25 2027 GMT
  host: imgapi.ai
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Imgapi Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ImgAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ImgAPI
provider_slug: imgapi-ai
slug: imgapi-ai-domain-security
source_filename: imgapi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imgapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 14:04:25 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: imgapi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/imgapi-ai/security/imgapi-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Image Generation
- Text-to-Image
- Image-to-Image
- Model Comparison
---
