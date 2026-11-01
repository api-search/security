---
api_specs:
- filename: intentdocs-com-cli-api-openapi.yml
  format: yaml
  label: intentdocs-com CLI API
  slug: intentdocs-com-cli-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-cli-api-openapi.yml
- filename: intentdocs-com-mcp-api-openapi.yml
  format: yaml
  label: intentdocs-com MCP API
  slug: intentdocs-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-mcp-api-openapi.yml
- filename: intentdocs-com-oauth-api-openapi.yml
  format: yaml
  label: intentdocs-com OAuth API
  slug: intentdocs-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-oauth-api-openapi.yml
- filename: intentdocs-com-sync-api-openapi.yml
  format: yaml
  label: intentdocs-com Sync API
  slug: intentdocs-com-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-sync-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intentdocs.com
  spf: true
hosts:
- cert_expires: Jan  8 18:05:35 2027 GMT
  host: intentdocs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intentdocs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for intentdocs-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: intentdocs-com
provider_slug: intentdocs-com
slug: intentdocs-com-domain-security
source_filename: intentdocs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intentdocs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 18:05:35 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: intentdocs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/intentdocs-com/security/intentdocs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Spec-Driven
- Platform
- Automation
- Low-Code
---
