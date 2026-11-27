---
api_specs:
- filename: facesign-ai-avatars-api-openapi.yml
  format: yaml
  label: FaceSign Avatars API
  slug: facesign-ai-avatars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facesign-ai/openapi/facesign-ai-avatars-api-openapi.yml
- filename: facesign-ai-langs-api-openapi.yml
  format: yaml
  label: FaceSign Langs API
  slug: facesign-ai-langs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facesign-ai/openapi/facesign-ai-langs-api-openapi.yml
- filename: facesign-ai-sessions-api-openapi.yml
  format: yaml
  label: FaceSign Sessions API
  slug: facesign-ai-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facesign-ai/openapi/facesign-ai-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: facesign.ai
  spf: true
hosts:
- cert_expires: Jan  3 12:59:43 2027 GMT
  host: facesign.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FaceSign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FaceSign, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FaceSign
provider_slug: facesign-ai
slug: facesign-ai-domain-security
source_filename: facesign-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: facesign.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 12:59:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: facesign.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/facesign-ai/security/facesign-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Identity Verification
- Deepfake Detection
- Liveness Detection
- Biometrics
---
