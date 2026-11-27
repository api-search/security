---
api_specs:
- filename: confcall-app-artifacts-api-openapi.yml
  format: yaml
  label: confcall Artifacts API
  slug: confcall-app-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-artifacts-api-openapi.yml
- filename: confcall-app-embed-api-openapi.yml
  format: yaml
  label: confcall Embed API
  slug: confcall-app-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-embed-api-openapi.yml
- filename: confcall-app-recordings-api-openapi.yml
  format: yaml
  label: confcall Recordings API
  slug: confcall-app-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-recordings-api-openapi.yml
- filename: confcall-app-rooms-api-openapi.yml
  format: yaml
  label: confcall Rooms API
  slug: confcall-app-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-rooms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: confcall.app
  spf: false
hosts:
- cert_expires: Dec  4 19:36:06 2026 GMT
  host: confcall.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: confcall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for confcall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: confcall
provider_slug: confcall-app
slug: confcall-app-domain-security
source_filename: confcall-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: confcall.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 19:36:06 2026 GMT\n  hsts: false\ndomains:\n- domain: confcall.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/confcall-app/security/confcall-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Video Conferencing
- AI Agents
- Embeddable Widgets
- Telephony
- Transcription
- MCP
- Communications
---
