---
api_key_in: []
auth_types:
- apiKey
description: Kosmos AI Labs exposes one authenticated public API — the OTLP ingest endpoint — secured with a static API key in a custom header. There is no public OAuth authorization server, no /.well-known/openid-configuration and no token endpoint of its own; OAuth appears only on the inbound side, where Kosmos acts as an OAuth *client* against the third-party systems a customer connects.
kind: authentication
layout: security
method: searched
name: Kosmoslabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kosmos AI Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kosmos AI Labs
provider_slug: kosmoslabs
scheme_count: 1
schemes:
- applies_to:
  - https://ingest.kosmoslabs.ai/v1/traces
  - https://ingest.kosmoslabs.ai/v1/metrics
  - https://ingest.kosmoslabs.ai/v1/logs
  description: API key generated in Kosmos platform settings and sent on every OTLP request. Keys are prefixed kos_.
  header_name: X-Kosmos-API-Key
  in: header
  key_prefix: kos_
  name: kosmosApiKey
  source: https://docs.kosmoslabs.ai/product-documentation/connecting-opentelemetry-preview
  transport:
  - OTLP over HTTP (primary)
  - OTLP over gRPC (alternative; header passed as gRPC metadata)
  type: apiKey
  verified:
    body: '{"code":401,"message":"missing API key"}'
    probe: POST https://ingest.kosmoslabs.ai/v1/traces with no key
    probed: '2026-07-19'
    status: 401
slug: kosmoslabs-authentication
source_filename: kosmoslabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://docs.kosmoslabs.ai/product-documentation/connecting-opentelemetry-preview and\n  https://docs.kosmoslabs.ai/product-documentation/integration-permissions — Kosmos publishes no\n  OpenAPI, so this profile is transcribed from the documentation and confirmed against a live\n  unauthenticated probe of the ingest endpoint.\ndocs: https://docs.kosmoslabs.ai/product-documentation/integration-permissions\ndescription: >-\n  Kosmos AI Labs exposes one authenticated public API — the OTLP ingest endpoint — secured with a\n  static API key in a custom header. There is no public OAuth authorization server, no\n  /.well-known/openid-configuration and no token endpoint of its own; OAuth appears only on the\n  inbound side, where Kosmos acts as an OAuth *client* against the third-party systems a customer\n  connects.\n\nsummary:\n  types:\n  - apiKey\n  oauth_authorization_server: false\n  openid_connect: false\n  mutual_tls:\
  \ false\n\nschemes:\n- name: kosmosApiKey\n  type: apiKey\n  in: header\n  header_name: X-Kosmos-API-Key\n  key_prefix: kos_\n  description: >-\n    API key generated in Kosmos platform settings and sent on every OTLP request. Keys are\n    prefixed kos_.\n  applies_to:\n  - https://ingest.kosmoslabs.ai/v1/traces\n  - https://ingest.kosmoslabs.ai/v1/metrics\n  - https://ingest.kosmoslabs.ai/v1/logs\n  transport:\n  - OTLP over HTTP (primary)\n  - OTLP over gRPC (alternative; header passed as gRPC metadata)\n  verified:\n    probe: POST https://ingest.kosmoslabs.ai/v1/traces with no key\n    status: 401\n    body: '{\"code\":401,\"message\":\"missing API key\"}'\n    probed: '2026-07-19'\n  source: https://docs.kosmoslabs.ai/product-documentation/connecting-opentelemetry-preview\n\n# Kosmos as an OAuth CLIENT against customer-connected systems. These are not Kosmos's own\n# scopes — they are the read-only permissions Kosmos requests when a customer connects a system.\n# Captured verbatim\
  \ from the Integration Permissions page.\nintegration_authorization:\n  default_posture: Read-only integration scopes by default; OAuth 2.0 where the vendor supports it.\n  docs: https://docs.kosmoslabs.ai/product-documentation/integration-permissions\n  systems:\n  - system: Salesforce Service Cloud\n    auth: OAuth (managed package installation required)\n    permissions: [Read Cases, Read Case Comments, Read Case History, Read Incidents, Read Users]\n  - system: Jira\n    auth: OAuth 2.0\n    permissions: [Read Issues, Read Projects, Read Comments]\n    optional_permissions: [Write Issues]\n  - system: GitHub\n    auth: OAuth\n    permissions: [Read Commits, Read Pull Requests, 'Read Repositories (metadata)']\n  - system: Bitbucket\n    auth: OAuth\n    permissions: [Read Commits, Read Pull Requests, 'Read Repositories (metadata)']\n  - system: ServiceNow\n    auth: OAuth (supports custom field mapping)\n    permissions: [Read Incidents, Read Change Requests]\n  - system: Zendesk\n\
  \    auth: OAuth\n    permissions: [Read Tickets, Read Custom Fields]\n  - system: Linear\n    auth: OAuth 2.0\n    permissions: [Issues, State, Labels, Teams, Assignees, Relations, Attachments]\n    optional_permissions: [Comments]\n  - system: Azure DevOps\n    auth: OAuth 2.0 via Microsoft Entra\n    permissions: [Work Items, Work Item Types, Projects, Teams]\n    optional_permissions: [Comments]\n  - system: Pylon\n    auth: API key authentication\n    permissions: [Read Issues]\n    optional_permissions: [Read Messages]\n  - system: OpenTelemetry\n    auth: API key authentication (generated in Kosmos settings)\n    permissions: [Traces ingestion, Logs ingestion, Metrics ingestion]\n  - system: Slack / Microsoft Teams\n    auth: OAuth / webhook authorization\n    permissions: [Post Messages]\n    note: Delivery channel only, not a signal source.\n\ntransport_security:\n  tls: TLS 1.2+ for data in transit\n  source: https://kosmoslabs.ai/resources/security/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kosmoslabs/refs/heads/main/authentication/kosmoslabs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Operational Intelligence
- Observability
- OpenTelemetry
- Incident Management
- Root Cause Analysis
- AIOps
- Enterprise Software
---
