---
api_specs:
- filename: norric-io-health-api-openapi.yml
  format: yaml
  label: Norric Health API
  slug: norric-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-health-api-openapi.yml
- filename: norric-io-intelligence-rest-api-openapi.yml
  format: yaml
  label: Norric Intelligence REST API
  slug: norric-io-intelligence-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-intelligence-rest-api-openapi.yml
- filename: norric-io-mcp-api-openapi.yml
  format: yaml
  label: Norric MCP API
  slug: norric-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-mcp-api-openapi.yml
- filename: norric-io-paid-danish-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Danish company intelligence API
  slug: norric-io-paid-danish-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-danish-company-intelligence-api-openapi.yml
- filename: norric-io-paid-estonian-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Estonian company intelligence API
  slug: norric-io-paid-estonian-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-estonian-company-intelligence-api-openapi.yml
- filename: norric-io-paid-finnish-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Finnish company intelligence API
  slug: norric-io-paid-finnish-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-finnish-company-intelligence-api-openapi.yml
- filename: norric-io-paid-french-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid French company intelligence API
  slug: norric-io-paid-french-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-french-company-intelligence-api-openapi.yml
- filename: norric-io-paid-norwegian-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Norwegian company intelligence API
  slug: norric-io-paid-norwegian-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-norwegian-company-intelligence-api-openapi.yml
- filename: norric-io-paid-swedish-company-intelligence-api-openapi.yml
  format: yaml
  label: Norric Paid Swedish company intelligence API
  slug: norric-io-paid-swedish-company-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-paid-swedish-company-intelligence-api-openapi.yml
- filename: norric-io-service-api-openapi.yml
  format: yaml
  label: Norric Service API
  slug: norric-io-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norric-io/openapi/norric-io-service-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: norric.io
  spf: true
hosts:
- cert_expires: Jan 14 14:43:24 2027 GMT
  host: norric.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Norric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Norric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Norric
provider_slug: norric-io
slug: norric-io-domain-security
source_filename: norric-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: norric.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 14:43:24 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: norric.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/norric-io/security/norric-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- EU
- Artificial Intelligence
- Registers
---
