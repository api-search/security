---
api_specs:
- filename: maketa-pro-agent-api-openapi.yml
  format: yaml
  label: Maketa Agent API
  slug: maketa-pro-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-agent-api-openapi.yml
- filename: maketa-pro-boards-api-openapi.yml
  format: yaml
  label: Maketa Boards API
  slug: maketa-pro-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-boards-api-openapi.yml
- filename: maketa-pro-keys-api-openapi.yml
  format: yaml
  label: Maketa Keys API
  slug: maketa-pro-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-keys-api-openapi.yml
- filename: maketa-pro-misc-api-openapi.yml
  format: yaml
  label: Maketa Misc API
  slug: maketa-pro-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-misc-api-openapi.yml
- filename: maketa-pro-screens-api-openapi.yml
  format: yaml
  label: Maketa Screens API
  slug: maketa-pro-screens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maketa-pro/openapi/maketa-pro-screens-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: maketa.pro
  spf: true
hosts:
- cert_expires: Jan 29 18:37:03 2027 GMT
  host: maketa.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Maketa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maketa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Maketa
provider_slug: maketa-pro
slug: maketa-pro-domain-security
source_filename: maketa-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maketa.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 18:37:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maketa.pro\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/maketa-pro/security/maketa-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- No-Code
- Prototyping
- Screen-Constructor
- AI-assisted
- Mockup
---
