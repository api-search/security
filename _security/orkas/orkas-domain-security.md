---
api_specs:
- filename: orkas-audio-api-openapi.yml
  format: yaml
  label: Orkas Audio API
  slug: orkas-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-audio-api-openapi.yml
- filename: orkas-images-api-openapi.yml
  format: yaml
  label: Orkas Images API
  slug: orkas-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-images-api-openapi.yml
- filename: orkas-openapi-json-api-openapi.yml
  format: yaml
  label: Orkas Openapi.json API
  slug: orkas-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-openapi-json-api-openapi.yml
- filename: orkas-search-api-openapi.yml
  format: yaml
  label: Orkas Search API
  slug: orkas-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-search-api-openapi.yml
- filename: orkas-videos-api-openapi.yml
  format: yaml
  label: Orkas Videos API
  slug: orkas-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-videos-api-openapi.yml
- filename: orkas-chat-completions-api-openapi.yml
  format: yaml
  label: Orkas Chat Completions API
  slug: orkas-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orkas.ai
  spf: true
hosts:
- cert_expires: Dec  5 12:02:56 2026 GMT
  host: orkas.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orkas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orkas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Orkas
provider_slug: orkas
slug: orkas-domain-security
source_filename: orkas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orkas.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 12:02:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: orkas.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/security/orkas-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Chatbots
- Media
---
