---
api_key_in: []
api_specs:
- filename: observeai-reporting-apis-openapi.yml
  format: yaml
  label: Observe.AI Reporting APIs
  slug: observeai-reporting-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/openapi/observeai-reporting-apis-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Observeai Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Observe.AI secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Observe.AI
provider_slug: observeai
scheme_count: 2
schemes:
- applied_to:
  - POST /v1/dsr/delete/on-demand
  - GET /v1/dsr/delete/{job_id}/status
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/observeai-reporting-apis-openapi.yml
  type: http
- credentials:
  - app_id
  - app_secret
  flow: clientCredentials
  name: OAuth2 App Credentials
  request_body_schema: OauthTokenRequest
  response_schema: OauthTokenResponse
  source: https://api-docs.observe.ai/#tag/Authentication
  token_endpoint: /v1/oauth/token
  token_operation: Create Auth Token
  type: oauth2
slug: observeai-authentication
source_filename: observeai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/observeai-reporting-apis-openapi.yml\ndocs: https://api-docs.observe.ai/#tag/Authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\nmodel: >-\n  Observe.AI Reporting APIs use an OAuth 2.0 \"App Credentials\" (client\n  credentials) flow. A customer generates an App ID and App Secret in the\n  Observe.AI application (maximum 3 apps per account), exchanges them at\n  POST /v1/oauth/token for a bearer JWT, and passes that token as\n  \"Authorization: Bearer <auth_token>\" on every reporting call. Basic Auth was\n  the legacy scheme and Observe.AI asked all clients to migrate off it by\n  31-Dec-2022.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied_to:\n  - POST /v1/dsr/delete/on-demand\n  - GET /v1/dsr/delete/{job_id}/status\n  sources:\n  - openapi/observeai-reporting-apis-openapi.yml\n- name: OAuth2 App Credentials\n\
  \  type: oauth2\n  flow: clientCredentials\n  token_endpoint: /v1/oauth/token\n  token_operation: Create Auth Token\n  credentials:\n  - app_id\n  - app_secret\n  request_body_schema: OauthTokenRequest\n  response_schema: OauthTokenResponse\n  source: https://api-docs.observe.ai/#tag/Authentication\ntoken:\n  type: JWT bearer\n  header: 'Authorization: Bearer <auth_token>'\n  lifetime_seconds: 7200\n  lifetime_note: Access token expires in 2 hours and must be re-created after expiry.\n  refresh: none — re-run the client-credentials exchange\ncredential_provisioning:\n  self_serve: false\n  process: >-\n    App credentials are requested from Observe.AI (help@observe.ai or the\n    customer's CSM) and generated in the application. The App ID and App Secret\n    are downloadable exactly once and cannot be viewed or re-downloaded later.\n  max_apps_per_account: 3\n  contact: help@observe.ai\nlegacy:\n  scheme: Basic Auth\n  status: deprecated\n  sunset_date: '2022-12-31'\n  note: >-\n    The\
  \ pre-2023 Calls Report API used HTTP Basic Auth. Observe.AI published a\n    migration notice asking all clients to move to OAuth 2.0 by 31-Dec-2022.\nspec_defects:\n- >-\n  components.securitySchemes in the published OpenAPI contains non-security\n  entries (DsrDeleteRequest, DsrRule, DsrDeleteResponse, DsrStatusResponse are\n  object schemas placed under securitySchemes rather than components.schemas).\n  Only bearerAuth is a real security scheme.\n- >-\n  The OAuth 2.0 client-credentials flow is documented in prose and modelled as a\n  plain POST operation; there is no oauth2 securityScheme declared in the spec,\n  so scopes/ is intentionally not emitted.\n- >-\n  There is no root-level `security:` and only the two DSR operations declare\n  `security: [bearerAuth]`; the 14 reporting operations require the same bearer\n  token per the docs but do not declare it in the spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/observeai/refs/heads/main/authentication/observeai-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Ai Apps
- Contact Center
- Conversation Intelligence
- Customer Support
- Agentic AI
- Voice AI
- Quality Assurance
- Reporting
- OpenAPI
- Speech Analytics
---
