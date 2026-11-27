---
api_specs:
- filename: creatica-app-backgrounds-api-openapi.yml
  format: yaml
  label: Creatica Backgrounds API
  slug: creatica-app-backgrounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-backgrounds-api-openapi.yml
- filename: creatica-app-generate-api-openapi.yml
  format: yaml
  label: Creatica Generate API
  slug: creatica-app-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-generate-api-openapi.yml
- filename: creatica-app-mcp-api-openapi.yml
  format: yaml
  label: Creatica MCP API
  slug: creatica-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-mcp-api-openapi.yml
- filename: creatica-app-palettes-api-openapi.yml
  format: yaml
  label: Creatica Palettes API
  slug: creatica-app-palettes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-palettes-api-openapi.yml
- filename: creatica-app-render-api-openapi.yml
  format: yaml
  label: Creatica Render API
  slug: creatica-app-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-render-api-openapi.yml
- filename: creatica-app-suggest-api-openapi.yml
  format: yaml
  label: Creatica Suggest API
  slug: creatica-app-suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-suggest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: creatica.app
  spf: true
hosts:
- cert_expires: Jan 23 07:36:39 2027 GMT
  host: creatica.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Creatica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creatica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Creatica
provider_slug: creatica-app
slug: creatica-app-domain-security
source_filename: creatica-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creatica.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 07:36:39 2027 GMT\n  hsts: false\ndomains:\n- domain: creatica.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/creatica-app/security/creatica-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SVG
- Backgrounds
- Design Tools
- Image Generation
- Generative Art
- MCP
- CLI
- Open Source
---
