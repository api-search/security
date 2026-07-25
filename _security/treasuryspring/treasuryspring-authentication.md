---
api_key_in: []
api_specs:
- filename: treasuryspring-calendar-api-openapi.yml
  format: yaml
  label: TreasurySpring Calendar API
  slug: treasuryspring-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-calendar-api-openapi.yml
- filename: treasuryspring-cells-api-openapi.yml
  format: yaml
  label: TreasurySpring Cells API
  slug: treasuryspring-cells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-cells-api-openapi.yml
- filename: treasuryspring-entities-api-openapi.yml
  format: yaml
  label: TreasurySpring Entities API
  slug: treasuryspring-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-entities-api-openapi.yml
- filename: treasuryspring-event-checkpoints-api-openapi.yml
  format: yaml
  label: TreasurySpring Event Checkpoints API
  slug: treasuryspring-event-checkpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-event-checkpoints-api-openapi.yml
- filename: treasuryspring-events-api-openapi.yml
  format: yaml
  label: TreasurySpring Events API
  slug: treasuryspring-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-events-api-openapi.yml
- filename: treasuryspring-healthcheck-api-openapi.yml
  format: yaml
  label: TreasurySpring Healthcheck API
  slug: treasuryspring-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-healthcheck-api-openapi.yml
- filename: treasuryspring-holdings-api-openapi.yml
  format: yaml
  label: TreasurySpring Holdings API
  slug: treasuryspring-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-holdings-api-openapi.yml
- filename: treasuryspring-indications-api-openapi.yml
  format: yaml
  label: TreasurySpring Indications API
  slug: treasuryspring-indications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-indications-api-openapi.yml
- filename: treasuryspring-oauth-api-openapi.yml
  format: yaml
  label: TreasurySpring OAuth API
  slug: treasuryspring-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-oauth-api-openapi.yml
- filename: treasuryspring-obligor-exposure-api-openapi.yml
  format: yaml
  label: TreasurySpring Obligor Exposure API
  slug: treasuryspring-obligor-exposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-obligor-exposure-api-openapi.yml
- filename: treasuryspring-subscriptions-api-openapi.yml
  format: yaml
  label: TreasurySpring Subscriptions API
  slug: treasuryspring-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-subscriptions-api-openapi.yml
- filename: treasuryspring-tasks-api-openapi.yml
  format: yaml
  label: TreasurySpring Tasks API
  slug: treasuryspring-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-tasks-api-openapi.yml
- filename: treasuryspring-webhooks-api-openapi.yml
  format: yaml
  label: TreasurySpring Webhooks API
  slug: treasuryspring-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Treasuryspring Authentication
name_suffix: Authentication
oauth_flows: []
overview: TreasurySpring secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TreasurySpring
provider_slug: treasuryspring
scheme_count: 2
schemes:
- description: 'Base64-encoded `client_id:client_secret` (sent as `Authorization: Basic <base64>`). Used by the OAuth token-exchange endpoint.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/treasuryspring-openapi-original.json
  type: http
- description: 'API Key or OAuth access token (sent as `Authorization: Bearer <token>`).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/treasuryspring-openapi-original.json
  type: http
slug: treasuryspring-authentication
source_filename: treasuryspring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/treasuryspring-openapi-original.json\ndocs: https://docs.treasuryspring.com/\nnotes: >-\n  REST API uses OAuth 2.0 client-credentials: exchange base64 client_id:client_secret\n  (HTTP Basic) at POST /oauth/token for a Bearer access token (access_token,\n  expires_in, refresh_token). All other endpoints take Authorization: Bearer <token>\n  (an API Key or OAuth access token). The published MCP server uses the OAuth 2.0\n  authorization-code flow with PKCE backed by Auth0, and advertises Dynamic Client\n  Registration (RFC 7591) so clients need no pre-configured client_id.\noauth2:\n  grant_types: [client_credentials, authorization_code]\n  token_endpoint: https://api.treasuryspring.com/api/v1/oauth/token\n  pkce: true\n  dynamic_client_registration: true\n  identity_provider: Auth0\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Base64-encoded `client_id:client_secret`\
  \ (sent as `Authorization: Basic <base64>`).\n    Used by the OAuth token-exchange endpoint.'\n  sources:\n  - openapi/treasuryspring-openapi-original.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API Key or OAuth access token (sent as `Authorization: Bearer <token>`).'\n  sources:\n  - openapi/treasuryspring-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/authentication/treasuryspring-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Fintech
- Cash Management
- Treasury
- Investments
- Financial Services
- Fixed Term Funds
- Payments
- MCP
---
