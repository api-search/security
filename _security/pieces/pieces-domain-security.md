---
api_specs:
- filename: pieces-applications-api-openapi.yml
  format: yaml
  label: Pieces Applications API
  slug: pieces-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-applications-api-openapi.yml
- filename: pieces-assets-api-openapi.yml
  format: yaml
  label: Pieces Assets API
  slug: pieces-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-assets-api-openapi.yml
- filename: pieces-conversations-api-openapi.yml
  format: yaml
  label: Pieces Conversations API
  slug: pieces-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-conversations-api-openapi.yml
- filename: pieces-formats-api-openapi.yml
  format: yaml
  label: Pieces Formats API
  slug: pieces-formats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-formats-api-openapi.yml
- filename: pieces-models-api-openapi.yml
  format: yaml
  label: Pieces Models API
  slug: pieces-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-models-api-openapi.yml
- filename: pieces-qgpt-api-openapi.yml
  format: yaml
  label: Pieces QGPT API
  slug: pieces-qgpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-qgpt-api-openapi.yml
- filename: pieces-user-api-openapi.yml
  format: yaml
  label: Pieces User API
  slug: pieces-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-user-api-openapi.yml
- filename: pieces-well-known-api-openapi.yml
  format: yaml
  label: Pieces Well Known API
  slug: pieces-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pieces.app
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: pieces.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 04:35:55 2026 GMT
  host: docs.pieces.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pieces Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pieces, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pieces
provider_slug: pieces
slug: pieces-domain-security
source_filename: pieces-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pieces.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pieces.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 04:35:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pieces.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/security/pieces-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Developer Tools
- On-Device
- Local API
- Long-Term Memory
---
