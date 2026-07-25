---
api_specs:
- filename: synthesia-assets-api-openapi.yml
  format: yaml
  label: Synthesia Assets API
  slug: synthesia-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-assets-api-openapi.yml
- filename: synthesia-auditlogs-api-openapi.yml
  format: yaml
  label: Synthesia AuditLogs API
  slug: synthesia-auditlogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-auditlogs-api-openapi.yml
- filename: synthesia-dubbing-api-openapi.yml
  format: yaml
  label: Synthesia Dubbing API
  slug: synthesia-dubbing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-dubbing-api-openapi.yml
- filename: synthesia-templates-api-openapi.yml
  format: yaml
  label: Synthesia Templates API
  slug: synthesia-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-templates-api-openapi.yml
- filename: synthesia-translations-api-openapi.yml
  format: yaml
  label: Synthesia Translations API
  slug: synthesia-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-translations-api-openapi.yml
- filename: synthesia-videos-api-openapi.yml
  format: yaml
  label: Synthesia Videos API
  slug: synthesia-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-videos-api-openapi.yml
- filename: synthesia-webhooks-api-openapi.yml
  format: yaml
  label: Synthesia Webhooks API
  slug: synthesia-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/openapi/synthesia-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: synthesia.io
  spf: true
hosts:
- cert_expires: Aug 16 16:30:22 2026 GMT
  host: www.synthesia.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 06:26:44 2026 GMT
  host: docs.synthesia.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.synthesia.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synthesia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthesia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Synthesia
provider_slug: synthesia
slug: synthesia-domain-security
source_filename: synthesia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synthesia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 16:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.synthesia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 06:26:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.synthesia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: synthesia.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthesia/refs/heads/main/security/synthesia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Generative AI
- Video
- Avatars
- Text To Video
- Voices
- Dubbing
- Translation
- Templates
- Enterprise
- Learning
---
