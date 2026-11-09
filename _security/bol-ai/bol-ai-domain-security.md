---
api_specs:
- filename: bol-ai-billing-api-openapi.yml
  format: yaml
  label: Bol.ai Billing API
  slug: bol-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-billing-api-openapi.yml
- filename: bol-ai-bol-api-openapi.yml
  format: yaml
  label: Bol.ai Bol API
  slug: bol-ai-bol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-bol-api-openapi.yml
- filename: bol-ai-mcp-api-openapi.yml
  format: yaml
  label: Bol.ai MCP API
  slug: bol-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-mcp-api-openapi.yml
- filename: bol-ai-me-api-openapi.yml
  format: yaml
  label: Bol.ai Me API
  slug: bol-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-me-api-openapi.yml
- filename: bol-ai-usage-api-openapi.yml
  format: yaml
  label: Bol.ai Usage API
  slug: bol-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-ai/openapi/bol-ai-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bol.ai
  spf: true
hosts:
- cert_expires: Jan  5 07:22:58 2027 GMT
  host: bol.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bol Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bol.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Bol.ai
provider_slug: bol-ai
slug: bol-ai-domain-security
source_filename: bol-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bol.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 07:22:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bol.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bol-ai/security/bol-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Freight Documents
- Data Extraction
- Bill of Lading
- 3PL
---
