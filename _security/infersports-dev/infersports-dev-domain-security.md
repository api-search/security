---
api_specs:
- filename: infersports-dev-convert-api-openapi.yml
  format: yaml
  label: InferSports Convert API
  slug: infersports-dev-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infersports-dev/openapi/infersports-dev-convert-api-openapi.yml
- filename: infersports-dev-events-api-openapi.yml
  format: yaml
  label: InferSports Events API
  slug: infersports-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infersports-dev/openapi/infersports-dev-events-api-openapi.yml
- filename: infersports-dev-mcp-api-openapi.yml
  format: yaml
  label: InferSports MCP API
  slug: infersports-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infersports-dev/openapi/infersports-dev-mcp-api-openapi.yml
- filename: infersports-dev-metadata-api-openapi.yml
  format: yaml
  label: InferSports Metadata API
  slug: infersports-dev-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infersports-dev/openapi/infersports-dev-metadata-api-openapi.yml
- filename: infersports-dev-odds-api-openapi.yml
  format: yaml
  label: InferSports Odds API
  slug: infersports-dev-odds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infersports-dev/openapi/infersports-dev-odds-api-openapi.yml
- filename: infersports-dev-ops-api-openapi.yml
  format: yaml
  label: InferSports Ops API
  slug: infersports-dev-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infersports-dev/openapi/infersports-dev-ops-api-openapi.yml
- filename: infersports-dev-platform-api-openapi.yml
  format: yaml
  label: InferSports Platform API
  slug: infersports-dev-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infersports-dev/openapi/infersports-dev-platform-api-openapi.yml
- filename: infersports-dev-resolve-api-openapi.yml
  format: yaml
  label: InferSports Resolve API
  slug: infersports-dev-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infersports-dev/openapi/infersports-dev-resolve-api-openapi.yml
- filename: infersports-dev-results-api-openapi.yml
  format: yaml
  label: InferSports Results API
  slug: infersports-dev-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infersports-dev/openapi/infersports-dev-results-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infersports.dev
  spf: true
hosts:
- cert_expires: Jan  1 05:54:54 2027 GMT
  host: infersports.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InferSports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InferSports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InferSports
provider_slug: infersports-dev
slug: infersports-dev-domain-security
source_filename: infersports-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infersports.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 05:54:54 2027 GMT\n  hsts: false\ndomains:\n- domain: infersports.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/infersports-dev/security/infersports-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Odds API
- Asian handicap
- Developer Tools
- Real-Time Data
---
