---
api_specs:
- filename: hedgr-app-health-api-openapi.yml
  format: yaml
  label: HEDGR Health API
  slug: hedgr-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-health-api-openapi.yml
- filename: hedgr-app-mcp-api-openapi.yml
  format: yaml
  label: HEDGR MCP API
  slug: hedgr-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-mcp-api-openapi.yml
- filename: hedgr-app-oauth-discovery-api-openapi.yml
  format: yaml
  label: HEDGR OAuth discovery API
  slug: hedgr-app-oauth-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-oauth-discovery-api-openapi.yml
- filename: hedgr-app-partner-api-api-openapi.yml
  format: yaml
  label: HEDGR Partner API
  slug: hedgr-app-partner-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-partner-api-api-openapi.yml
- filename: hedgr-app-rates-api-openapi.yml
  format: yaml
  label: HEDGR Rates API
  slug: hedgr-app-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-rates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hedgr.app
  spf: true
hosts:
- cert_expires: Dec 17 20:41:35 2026 GMT
  host: hedgr.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HEDGR Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HEDGR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HEDGR
provider_slug: hedgr-app
slug: hedgr-app-domain-security
source_filename: hedgr-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hedgr.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 20:41:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hedgr.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hedgr-app/security/hedgr-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Artificial Intelligence
- Foreign Exchange
- Small Business
- Accounting
- Platform
---
