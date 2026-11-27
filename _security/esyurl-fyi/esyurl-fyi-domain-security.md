---
api_specs:
- filename: esyurl-fyi-auth-api-openapi.yml
  format: yaml
  label: esyURL Auth API
  slug: esyurl-fyi-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-auth-api-openapi.yml
- filename: esyurl-fyi-domain-api-openapi.yml
  format: yaml
  label: esyURL Domain API
  slug: esyurl-fyi-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-domain-api-openapi.yml
- filename: esyurl-fyi-groups-api-openapi.yml
  format: yaml
  label: esyURL Groups API
  slug: esyurl-fyi-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-groups-api-openapi.yml
- filename: esyurl-fyi-links-api-openapi.yml
  format: yaml
  label: esyURL Links API
  slug: esyurl-fyi-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-links-api-openapi.yml
- filename: esyurl-fyi-mcp-api-openapi.yml
  format: yaml
  label: esyURL MCP API
  slug: esyurl-fyi-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-mcp-api-openapi.yml
- filename: esyurl-fyi-me-api-openapi.yml
  format: yaml
  label: esyURL Me API
  slug: esyurl-fyi-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-me-api-openapi.yml
- filename: esyurl-fyi-public-api-openapi.yml
  format: yaml
  label: esyURL Public API
  slug: esyurl-fyi-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-public-api-openapi.yml
- filename: esyurl-fyi-render-api-openapi.yml
  format: yaml
  label: esyURL Render API
  slug: esyurl-fyi-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esyurl-fyi/openapi/esyurl-fyi-render-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: esyurl.fyi
  spf: true
hosts:
- cert_expires: Dec 29 17:02:01 2026 GMT
  host: esyurl.fyi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: esyURL Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for esyURL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: esyURL
provider_slug: esyurl-fyi
slug: esyurl-fyi-domain-security
source_filename: esyurl-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: esyurl.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 17:02:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: esyurl.fyi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/esyurl-fyi/security/esyurl-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Short Links
- QR Codes
- AI Agents
- MCP
---
