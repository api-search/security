---
api_specs:
- filename: schemasure-health-api-openapi.yml
  format: yaml
  label: SchemaSure Health API
  slug: schemasure-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schemasure/refs/heads/main/openapi/schemasure-health-api-openapi.yml
- filename: schemasure-image-extraction-x402-v2-api-openapi.yml
  format: yaml
  label: SchemaSure Image extraction · x402 V2 API
  slug: schemasure-image-extraction-x402-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schemasure/refs/heads/main/openapi/schemasure-image-extraction-x402-v2-api-openapi.yml
- filename: schemasure-legacy-v1-evaluation-api-api-openapi.yml
  format: yaml
  label: SchemaSure Legacy V1 evaluation API
  slug: schemasure-legacy-v1-evaluation-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schemasure/refs/heads/main/openapi/schemasure-legacy-v1-evaluation-api-api-openapi.yml
- filename: schemasure-primary-x402-v2-api-api-openapi.yml
  format: yaml
  label: SchemaSure Primary x402 V2 API
  slug: schemasure-primary-x402-v2-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schemasure/refs/heads/main/openapi/schemasure-primary-x402-v2-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: schemasure.com
  spf: true
hosts:
- cert_expires: Oct 12 11:45:20 2026 GMT
  host: schemasure.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Schemasure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SchemaSure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SchemaSure
provider_slug: schemasure
slug: schemasure-domain-security
source_filename: schemasure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: schemasure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 11:45:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: schemasure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schemasure/refs/heads/main/security/schemasure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Structured Data Extraction
- text-to-JSON
- JSON-Schema
- Document Parsing
- Data Cleaning
- LLM Tooling
- AI Agents
- x402-micropayments
- agent-native
- A2A
- MCP
---
