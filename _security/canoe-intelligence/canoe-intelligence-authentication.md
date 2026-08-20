---
api_key_in: []
api_specs:
- filename: canoe-intelligence-allocations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Allocations API
  slug: canoe-intelligence-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-allocations-api-openapi.yml
- filename: canoe-intelligence-authentication-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Authentication API
  slug: canoe-intelligence-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-authentication-api-openapi.yml
- filename: canoe-intelligence-custom-fields-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Custom Fields API
  slug: canoe-intelligence-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-custom-fields-api-openapi.yml
- filename: canoe-intelligence-documents-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Documents API
  slug: canoe-intelligence-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-documents-api-openapi.yml
- filename: canoe-intelligence-funds-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Funds API
  slug: canoe-intelligence-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-funds-api-openapi.yml
- filename: canoe-intelligence-organizations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Organizations API
  slug: canoe-intelligence-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-organizations-api-openapi.yml
- filename: canoe-intelligence-password-grant-tokens-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Password Grant Tokens API
  slug: canoe-intelligence-password-grant-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-password-grant-tokens-api-openapi.yml
- filename: canoe-intelligence-terms-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Terms API
  slug: canoe-intelligence-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-terms-api-openapi.yml
- filename: canoe-intelligence-user-api-openapi.yml
  format: yaml
  label: Canoe Intelligence User API
  slug: canoe-intelligence-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-user-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Canoe Intelligence Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Canoe Intelligence secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Canoe Intelligence
provider_slug: canoe-intelligence
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Enter your Bearer token in the format: Bearer {token}'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/canoe-intelligence-api-openapi.yml
  type: http
- description: OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://api.canoesoftware.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.canoesoftware.com/oauth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.canoesoftware.com/v1/tokens
  name: oauth2
  sources:
  - openapi/canoe-intelligence-api-openapi.yml
  type: oauth2
slug: canoe-intelligence-authentication
source_filename: canoe-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource:\n- openapi/canoe-intelligence-api-openapi.yml\n- https://api.canoesoftware.com/docs\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  default_security: 'bearerAuth (applied at the OpenAPI document root; token endpoints opt out with security: [])'\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Enter your Bearer token in the format: Bearer {token}'\n  sources:\n  - openapi/canoe-intelligence-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.canoesoftware.com/oauth/authorize\n    tokenUrl: https://api.canoesoftware.com/oauth/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://api.canoesoftware.com/v1/tokens\n    scopes: 0\n  description: OAuth 2.0 authentication\n  sources:\n  - openapi/canoe-intelligence-api-openapi.yml\ndocs:\
  \ https://api.canoesoftware.com/docs\ntoken:\n  lifetime: 24 hours\n  type: JWT bearer\n  header: 'Authorization: Bearer {token}'\n  issuance_endpoints:\n  - operationId: RequestingTokensAuthCodes\n    path: /oauth/token\n    grant: authorization_code\n  - operationId: RequestingTokensRefreshToken\n    path: /oauth/token/refresh\n    grant: refresh_token\n  - operationId: RequestingTokensClientCredentials\n    path: /oauth/token/client-credentials\n    grant: client_credentials\n  - operationId: Tokens\n    path: /v1/tokens\n    grant: password\n    note: Takes API user credentials rather than a token — one of the few endpoints authenticated with user credentials.\n  authorize_url: https://api.canoesoftware.com/oauth/authorize\n  client_registration: https://client.canoesoftware.com/api_configuration\n  client_management_operation: ManageAuthClient (GET /oauth/clients)\nadditional_controls:\n- control: IP allowlisting\n  direction: inbound\n  note: Canoe can restrict which client IPs may\
  \ call the API, on request.\n- control: IP allowlisting\n  direction: outbound\n  note: Client networks may need to allowlist Canoe's published IP ranges; the list is in the authenticated knowledge\n    base.\n- control: Ports\n  note: The API uses ports 443 and 9443.\n- control: 'X-Requested-With: XMLHttpRequest'\n  note: Sent on every published code sample; treat as required.\nauthorization_model:\n  scopes: false\n  note: Both OAuth 2.0 flows declare an empty scopes map. Authorization is by purchased Canoe services plus per-user\n    permissions, surfaced as HTTP 403, not by OAuth scope.\nerrors:\n  artifact: errors/canoe-intelligence-problem-types.yml\n  codes:\n  - INVALID_CREDENTIALS\n  - MALFORMED_JWT\n  - RATE_LIMIT_EXCEEDED\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/authentication/canoe-intelligence-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Alternative Investments
- Private Markets
- Document Automation
- Data Extraction
- Fund Administration
- capital-calls
- k-1-tax-documents
- Portfolio Reporting
- Financial-Services
- Fintech
- Wealth Management
- Institutional Investors
---
