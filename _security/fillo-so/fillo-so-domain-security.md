---
api_specs:
- filename: fillo-so-agents-api-openapi.yml
  format: yaml
  label: Fillo Agents API
  slug: fillo-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-agents-api-openapi.yml
- filename: fillo-so-credentials-api-openapi.yml
  format: yaml
  label: Fillo Credentials API
  slug: fillo-so-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-credentials-api-openapi.yml
- filename: fillo-so-deliveries-api-openapi.yml
  format: yaml
  label: Fillo Deliveries API
  slug: fillo-so-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-deliveries-api-openapi.yml
- filename: fillo-so-fillo-management-api-api-openapi.yml
  format: yaml
  label: Fillo Fillo Management API
  slug: fillo-so-fillo-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-fillo-management-api-api-openapi.yml
- filename: fillo-so-forms-api-openapi.yml
  format: yaml
  label: Fillo Forms API
  slug: fillo-so-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-forms-api-openapi.yml
- filename: fillo-so-insights-api-openapi.yml
  format: yaml
  label: Fillo Insights API
  slug: fillo-so-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-insights-api-openapi.yml
- filename: fillo-so-integrations-api-openapi.yml
  format: yaml
  label: Fillo Integrations API
  slug: fillo-so-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-integrations-api-openapi.yml
- filename: fillo-so-members-api-openapi.yml
  format: yaml
  label: Fillo Members API
  slug: fillo-so-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-members-api-openapi.yml
- filename: fillo-so-respondents-api-openapi.yml
  format: yaml
  label: Fillo Respondents API
  slug: fillo-so-respondents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-respondents-api-openapi.yml
- filename: fillo-so-responses-api-openapi.yml
  format: yaml
  label: Fillo Responses API
  slug: fillo-so-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-responses-api-openapi.yml
- filename: fillo-so-settings-api-openapi.yml
  format: yaml
  label: Fillo Settings API
  slug: fillo-so-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-settings-api-openapi.yml
- filename: fillo-so-storage-api-openapi.yml
  format: yaml
  label: Fillo Storage API
  slug: fillo-so-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-storage-api-openapi.yml
- filename: fillo-so-webhooks-api-openapi.yml
  format: yaml
  label: Fillo Webhooks API
  slug: fillo-so-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-webhooks-api-openapi.yml
- filename: fillo-so-workspace-api-openapi.yml
  format: yaml
  label: Fillo Workspace API
  slug: fillo-so-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fillo-so/openapi/fillo-so-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fillo.so
  spf: true
hosts:
- cert_expires: Jan 13 12:33:36 2027 GMT
  host: fillo.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fillo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fillo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fillo
provider_slug: fillo-so
slug: fillo-so-domain-security
source_filename: fillo-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fillo.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 12:33:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fillo.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fillo-so/security/fillo-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Form Builder
- Developer Tools
- Embeddable Widgets
- Webhook
- Validation
- File Uploads
- SDK
- CLI
- Management API
---
