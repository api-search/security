---
api_specs:
- filename: anam-auth-api-openapi.yml
  format: yaml
  label: Anam Auth API
  slug: anam-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-auth-api-openapi.yml
- filename: anam-avatars-api-openapi.yml
  format: yaml
  label: Anam Avatars API
  slug: anam-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-avatars-api-openapi.yml
- filename: anam-knowledge-api-openapi.yml
  format: yaml
  label: Anam Knowledge API
  slug: anam-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-knowledge-api-openapi.yml
- filename: anam-llms-api-openapi.yml
  format: yaml
  label: Anam Llms API
  slug: anam-llms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-llms-api-openapi.yml
- filename: anam-personas-api-openapi.yml
  format: yaml
  label: Anam Personas API
  slug: anam-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-personas-api-openapi.yml
- filename: anam-sessions-api-openapi.yml
  format: yaml
  label: Anam Sessions API
  slug: anam-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-sessions-api-openapi.yml
- filename: anam-share-links-api-openapi.yml
  format: yaml
  label: Anam Share Links API
  slug: anam-share-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-share-links-api-openapi.yml
- filename: anam-tools-api-openapi.yml
  format: yaml
  label: Anam Tools API
  slug: anam-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-tools-api-openapi.yml
- filename: anam-voices-api-openapi.yml
  format: yaml
  label: Anam Voices API
  slug: anam-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-voices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anam.ai
  spf: true
hosts:
- cert_expires: Sep 15 19:51:51 2026 GMT
  host: www.anam.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anam
provider_slug: anam
slug: anam-domain-security
source_filename: anam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:51:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anam.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/security/anam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Avatars
- Conversational AI
- Video
- Real-Time
- Voice
- Agents
---
