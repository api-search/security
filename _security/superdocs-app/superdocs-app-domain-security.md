---
api_specs:
- filename: superdocs-app-account-api-openapi.yml
  format: yaml
  label: superdocs-app Account API
  slug: superdocs-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-account-api-openapi.yml
- filename: superdocs-app-agents-api-openapi.yml
  format: yaml
  label: superdocs-app Agents API
  slug: superdocs-app-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-agents-api-openapi.yml
- filename: superdocs-app-approval-api-openapi.yml
  format: yaml
  label: superdocs-app Approval API
  slug: superdocs-app-approval-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-approval-api-openapi.yml
- filename: superdocs-app-attachments-api-openapi.yml
  format: yaml
  label: superdocs-app Attachments API
  slug: superdocs-app-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-attachments-api-openapi.yml
- filename: superdocs-app-chat-api-openapi.yml
  format: yaml
  label: superdocs-app Chat API
  slug: superdocs-app-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-chat-api-openapi.yml
- filename: superdocs-app-documents-api-openapi.yml
  format: yaml
  label: superdocs-app Documents API
  slug: superdocs-app-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-documents-api-openapi.yml
- filename: superdocs-app-downloads-api-openapi.yml
  format: yaml
  label: superdocs-app Downloads API
  slug: superdocs-app-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-downloads-api-openapi.yml
- filename: superdocs-app-health-api-openapi.yml
  format: yaml
  label: superdocs-app Health API
  slug: superdocs-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-health-api-openapi.yml
- filename: superdocs-app-jobs-api-openapi.yml
  format: yaml
  label: superdocs-app Jobs API
  slug: superdocs-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-jobs-api-openapi.yml
- filename: superdocs-app-mcp-api-openapi.yml
  format: yaml
  label: superdocs-app MCP API
  slug: superdocs-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-mcp-api-openapi.yml
- filename: superdocs-app-promo-api-openapi.yml
  format: yaml
  label: superdocs-app Promo API
  slug: superdocs-app-promo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-promo-api-openapi.yml
- filename: superdocs-app-sessions-api-openapi.yml
  format: yaml
  label: superdocs-app Sessions API
  slug: superdocs-app-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-sessions-api-openapi.yml
- filename: superdocs-app-templates-api-openapi.yml
  format: yaml
  label: superdocs-app Templates API
  slug: superdocs-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-templates-api-openapi.yml
- filename: superdocs-app-typebar-api-universal-document-ai-api-openapi.yml
  format: yaml
  label: 'superdocs-app Typebar API: Universal Document AI API'
  slug: superdocs-app-typebar-api-universal-document-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-typebar-api-universal-document-ai-api-openapi.yml
- filename: superdocs-app-uploads-api-openapi.yml
  format: yaml
  label: superdocs-app Uploads API
  slug: superdocs-app-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-uploads-api-openapi.yml
- filename: superdocs-app-users-api-openapi.yml
  format: yaml
  label: superdocs-app Users API
  slug: superdocs-app-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-users-api-openapi.yml
- filename: superdocs-app-well-known-api-openapi.yml
  format: yaml
  label: superdocs-app .well Known API
  slug: superdocs-app-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superdocs-app/openapi/superdocs-app-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superdocs.app
  spf: true
hosts:
- cert_expires: Dec 10 10:44:11 2026 GMT
  host: superdocs.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Superdocs App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for superdocs-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: superdocs-app
provider_slug: superdocs-app
slug: superdocs-app-domain-security
source_filename: superdocs-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superdocs.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 10:44:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: superdocs.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/superdocs-app/security/superdocs-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Document Editing
- REST API
- MCP
- SaaS
---
