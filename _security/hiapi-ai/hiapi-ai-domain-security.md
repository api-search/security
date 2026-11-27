---
api_specs:
- filename: hiapi-ai-openapi-generated.yml
  format: yaml
  label: HiAPI API
  slug: hiapi-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hiapi-ai/openapi/_ae-authored/hiapi-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hiapi.ai
  spf: true
hosts:
- cert_expires: Feb  3 03:56:30 2027 GMT
  host: hiapi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HiAPI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HiAPI
provider_slug: hiapi-ai
slug: hiapi-ai-domain-security
source_filename: hiapi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hiapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 03:56:30 2027 GMT\n  hsts: false\ndomains:\n- domain: hiapi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hiapi-ai/security/hiapi-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Generative
- Image
- Video
- Audio
- Text
---
