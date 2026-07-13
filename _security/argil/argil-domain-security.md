---
api_specs:
- filename: argil-openapi.yml
  format: yaml
  label: Argil Videos API
  slug: argil-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
- filename: argil-openapi.yml
  format: yaml
  label: Argil Avatars API
  slug: argil-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
- filename: argil-openapi.yml
  format: yaml
  label: Argil Voices API
  slug: argil-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
- filename: argil-openapi.yml
  format: yaml
  label: Argil Assets API
  slug: argil-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
- filename: argil-openapi.yml
  format: yaml
  label: Argil Webhooks API
  slug: argil-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/openapi/argil-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: argil.ai
  spf: true
hosts:
- cert_expires: Oct  2 04:11:26 2026 GMT
  host: www.argil.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:06:10 2026 GMT
  host: docs.argil.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 10:13:36 2026 GMT
  host: api.argil.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argil, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Argil
provider_slug: argil
slug: argil-domain-security
source_filename: argil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.argil.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:11:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.argil.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:06:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.argil.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 10:13:36 2026 GMT\n  hsts: null\ndomains:\n- domain: argil.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argil/refs/heads/main/security/argil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Video Generation
- Avatars
- Voice Cloning
- Content Automation
---
