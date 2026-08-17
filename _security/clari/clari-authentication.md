---
api_key_in:
- header
api_specs:
- filename: clari-copilot-api-openapi.yml
  format: yaml
  label: Clari Copilot API
  slug: clari-copilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-copilot-api-openapi.yml
- filename: clari-activity-api-api-openapi.yml
  format: yaml
  label: Clari Activity API API
  slug: clari-activity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-activity-api-api-openapi.yml
- filename: clari-administrative-api-api-openapi.yml
  format: yaml
  label: Clari Administrative API API
  slug: clari-administrative-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-administrative-api-api-openapi.yml
- filename: clari-audit-api-api-openapi.yml
  format: yaml
  label: Clari Audit API API
  slug: clari-audit-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-audit-api-api-openapi.yml
- filename: clari-bulk-export-framework-api-openapi.yml
  format: yaml
  label: Clari Bulk Export Framework API
  slug: clari-bulk-export-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-export-framework-api-openapi.yml
- filename: clari-bulk-ingest-job-status-api-api-openapi.yml
  format: yaml
  label: Clari Bulk Ingest Job Status API API
  slug: clari-bulk-ingest-job-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-ingest-job-status-api-api-openapi.yml
- filename: clari-export-api-openapi.yml
  format: yaml
  label: Clari Export API
  slug: clari-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-export-api-openapi.yml
- filename: clari-forecast-api-api-openapi.yml
  format: yaml
  label: Clari Forecast API API
  slug: clari-forecast-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-forecast-api-api-openapi.yml
- filename: clari-ingestion-api-api-openapi.yml
  format: yaml
  label: Clari Ingestion API API
  slug: clari-ingestion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-ingestion-api-api-openapi.yml
- filename: clari-opportunity-api-api-openapi.yml
  format: yaml
  label: Clari Opportunity API API
  slug: clari-opportunity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-opportunity-api-api-openapi.yml
auth_types:
- apiKey
description: Clari runs three distinct authentication schemes across three surfaces. The Revenue API uses a single `apikey` header (plus a `partnerkey` header on partner/ingest endpoints). The Copilot REST API requires BOTH `X-Api-Key` and `X-Api-Password` — either alone returns 401. The MCP server uses OAuth 2.0 via Okta and is the only Clari surface with delegated authorization; see scopes/clari-scopes.yml.
kind: authentication
layout: security
method: searched
name: Clari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clari secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clari
provider_slug: clari
scheme_count: 3
schemes:
- in: header
  name: api_key
  parameter: apikey
  sources:
  - openapi/clari-activity-api-api-openapi.yml
  - openapi/clari-administrative-api-api-openapi.yml
  - openapi/clari-audit-api-api-openapi.yml
  - openapi/clari-bulk-export-framework-api-openapi.yml
  - openapi/clari-bulk-ingest-job-status-api-api-openapi.yml
  - openapi/clari-export-api-openapi.yml
  - openapi/clari-forecast-api-api-openapi.yml
  - openapi/clari-ingestion-api-api-openapi.yml
  - openapi/clari-opportunity-api-api-openapi.yml
  type: apiKey
- in: header
  name: api_key
  parameter: X-Api-Key
  sources:
  - openapi/clari-copilot-api-openapi.yml
  type: apiKey
- in: header
  name: api_password
  parameter: X-Api-Password
  sources:
  - openapi/clari-copilot-api-openapi.yml
  type: apiKey
slug: clari-authentication
source_filename: clari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs:\n- https://developer.clari.com/documentation/external_spec\n- https://api-doc.copilot.clari.com/\n- https://community.clari.com/product-q-a-6/how-to-use-copilot-apis-2258\ndescription: >-\n  Clari runs three distinct authentication schemes across three surfaces. The Revenue\n  API uses a single `apikey` header (plus a `partnerkey` header on partner/ingest\n  endpoints). The Copilot REST API requires BOTH `X-Api-Key` and `X-Api-Password` —\n  either alone returns 401. The MCP server uses OAuth 2.0 via Okta and is the only\n  Clari surface with delegated authorization; see scopes/clari-scopes.yml.\nissuance:\n  revenue_api:\n    location: Account Settings > API Token > \"Generate New API Token\"\n    caveats:\n    - The token value is displayed once and cannot be retrieved again.\n    - Revoking a token breaks every integration using it.\n    - Deactivating a user revokes every token that user created.\n    - A CSM must grant access\
  \ to the token generation tool if it is not visible.\n  copilot_api:\n    location: Workspace Settings > Integrations > Clari Copilot API\n    note: Yields both the key and the password.\n  mcp:\n    type: oauth2\n    authorization_endpoint: https://app.clari.com/authorize\n    issuer: https://clariciam.okta.com/oauth2/aus13shznanP7WOkp698\n    dynamic_client_registration: https://mcp.clari.com/okta/clients\n    see: scopes/clari-scopes.yml\nsource: openapi/clari-activity-api-api-openapi.yml, openapi/clari-administrative-api-api-openapi.yml,\n  openapi/clari-audit-api-api-openapi.yml, openapi/clari-bulk-export-framework-api-openapi.yml,\n  openapi/clari-bulk-ingest-job-status-api-api-openapi.yml, openapi/clari-copilot-api-openapi.yml,\n  openapi/clari-export-api-openapi.yml, openapi/clari-forecast-api-api-openapi.yml, openapi/clari-ingestion-api-api-openapi.yml,\n  openapi/clari-opportunity-api-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name:\
  \ api_key\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/clari-activity-api-api-openapi.yml\n  - openapi/clari-administrative-api-api-openapi.yml\n  - openapi/clari-audit-api-api-openapi.yml\n  - openapi/clari-bulk-export-framework-api-openapi.yml\n  - openapi/clari-bulk-ingest-job-status-api-api-openapi.yml\n  - openapi/clari-export-api-openapi.yml\n  - openapi/clari-forecast-api-api-openapi.yml\n  - openapi/clari-ingestion-api-api-openapi.yml\n  - openapi/clari-opportunity-api-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/clari-copilot-api-openapi.yml\n- name: api_password\n  type: apiKey\n  in: header\n  parameter: X-Api-Password\n  sources:\n  - openapi/clari-copilot-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/authentication/clari-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Revenue Operations
- Forecasting
- Pipeline Management
- Sales Intelligence
- Activity Intelligence
- Deal Insights
- CRM
- Conversation Intelligence
- B2B
- Enterprise
- MCP
- Agents
- Sales Engagement
- Bulk Export
- Data Ingestion
---
