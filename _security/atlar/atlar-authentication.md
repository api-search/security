---
anonymous_access: false
api_key_in: []
api_specs:
- filename: atlar-accounts-api-openapi.yml
  format: yaml
  label: Atlar Accounts API
  slug: atlar-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-accounts-api-openapi.yml
- filename: atlar-audit-logs-api-openapi.yml
  format: yaml
  label: Atlar Audit logs API
  slug: atlar-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-audit-logs-api-openapi.yml
- filename: atlar-connections-api-openapi.yml
  format: yaml
  label: Atlar Connections API
  slug: atlar-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-connections-api-openapi.yml
- filename: atlar-counterparties-api-openapi.yml
  format: yaml
  label: Atlar Counterparties API
  slug: atlar-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-counterparties-api-openapi.yml
- filename: atlar-credit-transfers-api-openapi.yml
  format: yaml
  label: Atlar Credit Transfers API
  slug: atlar-credit-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-credit-transfers-api-openapi.yml
- filename: atlar-direct-debits-api-openapi.yml
  format: yaml
  label: Atlar Direct Debits API
  slug: atlar-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-direct-debits-api-openapi.yml
- filename: atlar-documents-api-openapi.yml
  format: yaml
  label: Atlar Documents API
  slug: atlar-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-documents-api-openapi.yml
- filename: atlar-entities-api-openapi.yml
  format: yaml
  label: Atlar Entities API
  slug: atlar-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-entities-api-openapi.yml
- filename: atlar-events-webhooks-api-openapi.yml
  format: yaml
  label: Atlar Events (webhooks) API
  slug: atlar-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-events-webhooks-api-openapi.yml
- filename: atlar-external-accounts-api-openapi.yml
  format: yaml
  label: Atlar External Accounts API
  slug: atlar-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-external-accounts-api-openapi.yml
- filename: atlar-forecasted-transactions-api-openapi.yml
  format: yaml
  label: Atlar Forecasted Transactions API
  slug: atlar-forecasted-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-forecasted-transactions-api-openapi.yml
- filename: atlar-gl-accounts-api-openapi.yml
  format: yaml
  label: Atlar GL Accounts API
  slug: atlar-gl-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-gl-accounts-api-openapi.yml
- filename: atlar-gl-entities-api-openapi.yml
  format: yaml
  label: Atlar GL Entities API
  slug: atlar-gl-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-gl-entities-api-openapi.yml
- filename: atlar-investments-api-openapi.yml
  format: yaml
  label: Atlar Investments API
  slug: atlar-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-investments-api-openapi.yml
- filename: atlar-mandates-api-openapi.yml
  format: yaml
  label: Atlar Mandates API
  slug: atlar-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-mandates-api-openapi.yml
- filename: atlar-oauth-api-openapi.yml
  format: yaml
  label: Atlar OAuth API
  slug: atlar-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-oauth-api-openapi.yml
- filename: atlar-pending-transactions-api-openapi.yml
  format: yaml
  label: Atlar Pending Transactions API
  slug: atlar-pending-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-pending-transactions-api-openapi.yml
- filename: atlar-regulatory-reporting-api-openapi.yml
  format: yaml
  label: Atlar Regulatory Reporting API
  slug: atlar-regulatory-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-regulatory-reporting-api-openapi.yml
- filename: atlar-transactions-api-openapi.yml
  format: yaml
  label: Atlar Transactions API
  slug: atlar-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-transactions-api-openapi.yml
- filename: atlar-webhooks-api-openapi.yml
  format: yaml
  label: Atlar Webhooks API
  slug: atlar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/openapi/atlar-webhooks-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Atlar Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Atlar secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Atlar
provider_slug: atlar
scheme_count: 3
schemes:
- access_token_ttl_seconds: 300
  credentials: Programmatic access user ACCESS_KEY as client_id and SECRET as client_secret. Supports client_secret_basic and client_secret_post.
  name: OAuth2ClientCredentials
  recommended: true
  scheme: clientCredentials
  tokenUrl: https://api.atlar.com/iam/v2/oauth2/token
  token_endpoint_v2beta: https://api.atlar.com/iam/v2beta/oauth2/token
  token_type: Bearer
  type: oauth2
- authorizationUrl: https://api.atlar.com/iam/v2/oauth2/authorize
  name: OAuth2AuthorizationCode
  pkce: S256
  scheme: authorizationCode
  tokenUrl: https://api.atlar.com/iam/v2/oauth2/token
  type: oauth2
  used_for: MCP CIMD clients (mcp.atlar.com), plus refresh_token grant
- credentials: ACCESS_KEY as username, SECRET as password
  name: HTTPBasic
  note: Supported but OAuth 2.0 access-token flow is recommended
  scheme: basic
  type: http
slug: atlar-authentication
source_filename: atlar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.atlar.com/docs/api\ndocs: https://docs.atlar.com/docs/accessing-the-api\nsummary:\n  types: [oauth2, http]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  well_known: https://api.atlar.com/.well-known/oauth-authorization-server\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    scheme: clientCredentials\n    tokenUrl: https://api.atlar.com/iam/v2/oauth2/token\n    token_endpoint_v2beta: https://api.atlar.com/iam/v2beta/oauth2/token\n    token_type: Bearer\n    access_token_ttl_seconds: 300\n    credentials: >-\n      Programmatic access user ACCESS_KEY as client_id and SECRET as\n      client_secret. Supports client_secret_basic and client_secret_post.\n    recommended: true\n  - name: OAuth2AuthorizationCode\n    type: oauth2\n    scheme: authorizationCode\n    authorizationUrl: https://api.atlar.com/iam/v2/oauth2/authorize\n    tokenUrl: https://api.atlar.com/iam/v2/oauth2/token\n\
  \    pkce: S256\n    used_for: MCP CIMD clients (mcp.atlar.com), plus refresh_token grant\n  - name: HTTPBasic\n    type: http\n    scheme: basic\n    credentials: ACCESS_KEY as username, SECRET as password\n    note: Supported but OAuth 2.0 access-token flow is recommended\nnotes: >-\n  Bearer access tokens are passed as `Authorization: Bearer <token>`. Tokens are\n  short-lived (expires_in = 300s). Programmatic access users are created in the\n  Atlar Dashboard. Organizations gate agent/third-party OAuth via a Read-only or\n  Read-and-write access policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlar/refs/heads/main/authentication/atlar-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Fintech
- Treasury
- Payments
- Banking
- Cash Management
- Financial Operations
- ERP Integration
---
