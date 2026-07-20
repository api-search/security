---
api_specs:
- filename: amigo-classic-openapi-original.json
  format: json
  label: Amigo Classic API
  slug: amigo-classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amigo/refs/heads/main/openapi/amigo-classic-openapi-original.json
- filename: amigo-platform-openapi-original.json
  format: json
  label: Amigo Platform API
  slug: amigo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amigo/refs/heads/main/openapi/amigo-platform-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amigo.ai
  spf: true
hosts:
- cert_expires: Oct  8 23:57:26 2026 GMT
  host: docs.amigo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: api.amigo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.platform.amigo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amigo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amigo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amigo
provider_slug: amigo
slug: amigo-domain-security
source_filename: amigo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.amigo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:57:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.amigo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\n- host: api.platform.amigo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amigo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amigo/refs/heads/main/security/amigo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Healthcare
- AI Agents
- Voice
- Clinical
- Conversational AI
- FHIR
- EHR
- HIPAA
---
