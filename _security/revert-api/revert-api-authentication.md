---
api_key_in: []
api_specs:
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified CRM API
  slug: revert-api-unified-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified Chat API
  slug: revert-api-unified-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified Ticketing API
  slug: revert-api-unified-ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Connection Management API
  slug: revert-api-connection-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Metadata API
  slug: revert-api-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Passthrough Proxy API
  slug: revert-api-passthrough-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified Accounting API
  slug: revert-api-unified-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
- filename: revert-api-openapi.yml
  format: yaml
  label: Revert Unified ATS API
  slug: revert-api-unified-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/openapi/revert-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Revert Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revert secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Revert
provider_slug: revert-api
scheme_count: 3
schemes:
- description: Your Revert API key (private token), found on the Revert dashboard for an environment (Production or Sandbox). Sent on every request as the `x-revert-api-token` header. On self-hosted deployments this is the token of your own Revert instance.
  headerName: x-revert-api-token
  in: header
  name: revertApiToken
  sources:
  - openapi/revert-api-openapi.yml
  - https://github.com/revertinc/revert
  type: apiKey
- description: The tenant / customer id (t_id) captured when a customer linked their third-party account through the Revert connect flow. Required on unified data endpoints (CRM, chat, ticketing, accounting, ATS) and connection endpoints so Revert knows which linked connection and refreshed OAuth token to use.
  headerName: x-revert-t-id
  in: header
  name: revertTenantId
  sources:
  - openapi/revert-api-openapi.yml
  - https://github.com/revertinc/revert
  type: apiKey
- description: Optional Revert API version selector. If omitted, Revert defaults to the latest version of the API.
  headerName: x-api-version
  in: header
  name: revertApiVersion
  sources:
  - https://github.com/revertinc/revert
  type: apiKey
slug: revert-api-authentication
source_filename: revert-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/revert-api-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: revertApiToken\n  type: apiKey\n  in: header\n  headerName: x-revert-api-token\n  description: >-\n    Your Revert API key (private token), found on the Revert dashboard for an\n    environment (Production or Sandbox). Sent on every request as the\n    `x-revert-api-token` header. On self-hosted deployments this is the token of\n    your own Revert instance.\n  sources:\n  - openapi/revert-api-openapi.yml\n  - https://github.com/revertinc/revert\n- name: revertTenantId\n  type: apiKey\n  in: header\n  headerName: x-revert-t-id\n  description: >-\n    The tenant / customer id (t_id) captured when a customer linked their\n    third-party account through the Revert connect flow. Required on unified data\n    endpoints (CRM, chat, ticketing, accounting, ATS) and connection endpoints so\n    Revert knows which linked connection and refreshed OAuth token\
  \ to use.\n  sources:\n  - openapi/revert-api-openapi.yml\n  - https://github.com/revertinc/revert\n- name: revertApiVersion\n  type: apiKey\n  in: header\n  headerName: x-api-version\n  description: >-\n    Optional Revert API version selector. If omitted, Revert defaults to the\n    latest version of the API.\n  sources:\n  - https://github.com/revertinc/revert\nnotes: >-\n  Revert does not use OAuth bearer tokens for its own API - the end-user OAuth to\n  the downstream provider (Salesforce, HubSpot, Slack, Jira, etc.) is handled by\n  Revert during the connect flow, and Revert transparently refreshes those tokens.\n  The frontend connect SDK uses a separate public token (revertPublicToken) to\n  initiate a connection and to subscribe to the SSE connect-status stream; that\n  public token is not used to authorize server-side data calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revert-api/refs/heads/main/authentication/revert-api-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Unified API
- Embedded iPaaS
- Integrations
- Product Integrations
- Open Source
- CRM Integrations
- Connectors
- API Integration
---
