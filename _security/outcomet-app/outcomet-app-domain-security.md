---
api_specs:
- filename: outcomet-app-ask-api-openapi.yml
  format: yaml
  label: Outcomet Ask API
  slug: outcomet-app-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-ask-api-openapi.yml
- filename: outcomet-app-batch-api-openapi.yml
  format: yaml
  label: Outcomet Batch API
  slug: outcomet-app-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-batch-api-openapi.yml
- filename: outcomet-app-discovery-api-openapi.yml
  format: yaml
  label: Outcomet Discovery API
  slug: outcomet-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-discovery-api-openapi.yml
- filename: outcomet-app-mcp-api-openapi.yml
  format: yaml
  label: Outcomet MCP API
  slug: outcomet-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-mcp-api-openapi.yml
- filename: outcomet-app-onboarding-api-openapi.yml
  format: yaml
  label: Outcomet Onboarding API
  slug: outcomet-app-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-onboarding-api-openapi.yml
- filename: outcomet-app-sandbox-api-openapi.yml
  format: yaml
  label: Outcomet Sandbox API
  slug: outcomet-app-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-sandbox-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: outcomet.app
  spf: true
hosts:
- cert_expires: Jan 31 18:32:55 2027 GMT
  host: outcomet.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Outcomet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outcomet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Outcomet
provider_slug: outcomet-app
slug: outcomet-app-domain-security
source_filename: outcomet-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outcomet.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 18:32:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: outcomet.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/outcomet-app/security/outcomet-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Product Management
- Feedback
- Decision-Making
---
