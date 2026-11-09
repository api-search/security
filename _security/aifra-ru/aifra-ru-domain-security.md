---
api_specs:
- filename: aifra-ru-analytics-api-openapi.yml
  format: yaml
  label: AIfra Analytics API
  slug: aifra-ru-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-analytics-api-openapi.yml
- filename: aifra-ru-health-api-openapi.yml
  format: yaml
  label: AIfra Health API
  slug: aifra-ru-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-health-api-openapi.yml
- filename: aifra-ru-mcp-api-openapi.yml
  format: yaml
  label: AIfra MCP API
  slug: aifra-ru-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-mcp-api-openapi.yml
- filename: aifra-ru-previews-api-openapi.yml
  format: yaml
  label: AIfra Previews API
  slug: aifra-ru-previews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-previews-api-openapi.yml
- filename: aifra-ru-ready-api-openapi.yml
  format: yaml
  label: AIfra Ready API
  slug: aifra-ru-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-ready-api-openapi.yml
- filename: aifra-ru-remote-api-openapi.yml
  format: yaml
  label: AIfra Remote API
  slug: aifra-ru-remote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-remote-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: aifra.ru
  spf: true
hosts:
- cert_expires: Dec  7 17:27:14 2026 GMT
  host: aifra.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aifra Ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIfra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: AIfra
provider_slug: aifra-ru
slug: aifra-ru-domain-security
source_filename: aifra-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aifra.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 17:27:14 2026 GMT\n  hsts: false\ndomains:\n- domain: aifra.ru\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aifra-ru/security/aifra-ru-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Software-as-a-Service
- Static-Previews
- Artificial Intelligence
- CLI
- REST
---
