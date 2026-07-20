---
api_specs:
- filename: krisp-developers-openapi.yml
  format: yaml
  label: Krisp Voice Translation API
  slug: voice-translation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krisp/refs/heads/main/openapi/krisp-developers-openapi.yml
- filename: krisp-developers-openapi.yml
  format: yaml
  label: Krisp SDK & Model Downloads API
  slug: sdk-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krisp/refs/heads/main/openapi/krisp-developers-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: krisp.ai
  spf: true
hosts:
- cert_expires: Oct 15 14:28:52 2026 GMT
  host: krisp.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 09:00:42 2026 GMT
  host: api.developers.krisp.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:32:15 2026 GMT
  host: sdk-docs.krisp.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Krisp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Krisp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Krisp
provider_slug: krisp
slug: krisp-domain-security
source_filename: krisp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: krisp.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:28:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.developers.krisp.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:00:42 2026 GMT\n  hsts: null\n- host: sdk-docs.krisp.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:32:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: krisp.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/krisp/refs/heads/main/security/krisp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Voice AI
- Speech
- Audio
- Noise Cancellation
- Speech Translation
- Real Time Communications
- WebRTC
- Conversational AI
- SDK
- Machine Learning
---
