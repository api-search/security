---
api_key_in: []
api_specs:
- filename: remote-companies-api-openapi.yml
  format: yaml
  label: Remote Companies API
  slug: remote-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-companies-api-openapi.yml
- filename: remote-employments-api-openapi.yml
  format: yaml
  label: Remote Employments API
  slug: remote-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-employments-api-openapi.yml
- filename: remote-contractors-api-openapi.yml
  format: yaml
  label: Remote Contractors API
  slug: remote-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-contractors-api-openapi.yml
- filename: remote-payroll-billing-api-openapi.yml
  format: yaml
  label: Remote Payroll and Billing API
  slug: remote-payroll-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-payroll-billing-api-openapi.yml
- filename: remote-time-attendance-api-openapi.yml
  format: yaml
  label: Remote Time and Attendance API
  slug: remote-time-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-time-attendance-api-openapi.yml
- filename: remote-benefits-api-openapi.yml
  format: yaml
  label: Remote Benefits API
  slug: remote-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-benefits-api-openapi.yml
- filename: remote-files-api-openapi.yml
  format: yaml
  label: Remote Files and Custom Fields API
  slug: remote-files-and-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-files-api-openapi.yml
- filename: remote-oauth-api-openapi.yml
  format: yaml
  label: Remote OAuth 2.0 API
  slug: remote-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-oauth-api-openapi.yml
- filename: remote-webhooks-asyncapi.yml
  format: yaml
  label: Remote Webhooks
  slug: remote-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/asyncapi/remote-webhooks-asyncapi.yml
auth_types:
- oauth2
- http
description: 'Remote authenticates API calls with OAuth 2.0 bearer tokens (JWT). Resource endpoints present the token as an HTTP bearer (the BearerAuth scheme in every OpenAPI). Tokens are obtained through four flows: authorization code (customer apps and partners, with company consent), client credentials (partners across consented companies), JWT bearer assertion (partners acting for a specific company), and refresh token. A single authorization-request scope, https://gateway.remote.com/company.manage, is combined with a fine-grained read/write permission model (see scopes/). Customers can also mint a Customer API Token in the platform; a Client Token exists for marketing endpoints only.'
kind: authentication
layout: security
method: searched
name: Remote Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- jwt-bearer-assertion
- refreshToken
overview: Remote secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, jwt-bearer-assertion, and refreshToken flow(s).
provider_name: Remote
provider_slug: remote-com
scheme_count: 2
schemes:
- docs: https://developer.remote.com/docs/authentication
  flows:
    authorizationCode:
      authorizationUrl: https://gateway.remote.com/auth/oauth2/authorize
      scopes_ref: scopes/remote-com-scopes.yml
      tokenUrl: https://gateway.remote.com/auth/oauth2/token
    clientCredentials:
      tokenUrl: https://gateway.remote.com/auth/oauth2/token
    jwtBearerAssertion:
      grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
      tokenUrl: https://gateway.remote.com/auth/oauth2/token
    refreshToken:
      tokenUrl: https://gateway.remote.com/auth/oauth2/token
  name: OAuth2
  sandbox:
    authorizationUrl: https://gateway.remote-sandbox.com/auth/oauth2/authorize
    tokenUrl: https://gateway.remote-sandbox.com/auth/oauth2/token
  type: oauth2
- bearerFormat: JWT
  description: The access token from any OAuth flow is presented as an HTTP bearer on resource endpoints.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/remote-benefits-api-openapi.yml
  - openapi/remote-companies-api-openapi.yml
  - openapi/remote-contractors-api-openapi.yml
  - openapi/remote-employments-api-openapi.yml
  - openapi/remote-files-api-openapi.yml
  - openapi/remote-payroll-billing-api-openapi.yml
  - openapi/remote-time-attendance-api-openapi.yml
  type: http
slug: remote-com-authentication
source_filename: remote-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: >-\n  https://developer.remote.com/docs/authentication,\n  https://developer.remote.com/docs/authorization-code-flow,\n  https://developer.remote.com/docs/client-credentials-flow-for-partners,\n  https://developer.remote.com/docs/authorization-method-oauth-assertion,\n  https://developer.remote.com/docs/refresh-token-flow, upgrading the derived\n  OpenAPI securitySchemes (http bearer JWT) with the documented OAuth 2.0 model.\ndocs: https://developer.remote.com/docs/authentication\nsummary:\n  types: [oauth2, http]\n  http_bearer: JWT\n  oauth2_flows: [authorizationCode, clientCredentials, jwt-bearer-assertion, refreshToken]\ndescription: >-\n  Remote authenticates API calls with OAuth 2.0 bearer tokens (JWT). Resource\n  endpoints present the token as an HTTP bearer (the BearerAuth scheme in every\n  OpenAPI). Tokens are obtained through four flows: authorization code (customer\n  apps and partners, with company consent), client\
  \ credentials (partners across\n  consented companies), JWT bearer assertion (partners acting for a specific\n  company), and refresh token. A single authorization-request scope,\n  https://gateway.remote.com/company.manage, is combined with a fine-grained\n  read/write permission model (see scopes/). Customers can also mint a Customer\n  API Token in the platform; a Client Token exists for marketing endpoints only.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://gateway.remote.com/auth/oauth2/authorize\n        tokenUrl: https://gateway.remote.com/auth/oauth2/token\n        scopes_ref: scopes/remote-com-scopes.yml\n      clientCredentials:\n        tokenUrl: https://gateway.remote.com/auth/oauth2/token\n      jwtBearerAssertion:\n        grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n        tokenUrl: https://gateway.remote.com/auth/oauth2/token\n      refreshToken:\n        tokenUrl: https://gateway.remote.com/auth/oauth2/token\n\
  \    sandbox:\n      authorizationUrl: https://gateway.remote-sandbox.com/auth/oauth2/authorize\n      tokenUrl: https://gateway.remote-sandbox.com/auth/oauth2/token\n    docs: https://developer.remote.com/docs/authentication\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: The access token from any OAuth flow is presented as an HTTP bearer on resource endpoints.\n    sources:\n      - openapi/remote-benefits-api-openapi.yml\n      - openapi/remote-companies-api-openapi.yml\n      - openapi/remote-contractors-api-openapi.yml\n      - openapi/remote-employments-api-openapi.yml\n      - openapi/remote-files-api-openapi.yml\n      - openapi/remote-payroll-billing-api-openapi.yml\n      - openapi/remote-time-attendance-api-openapi.yml\ntoken_types:\n  - {name: Company-scoped access token, note: Scoped to a single company; returned on company creation and OAuth authorization.}\n  - {name: Partner token, note: Client-credentials token operating\
  \ across all companies that granted consent.}\n  - {name: Customer API Token, note: Generated in the Remote platform for user-authenticated requests.}\n  - {name: Client Token, note: Bearer token for marketing endpoints only; excludes sensitive-data access.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/authentication/remote-com-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Global Payroll
- EOR
- Contractor Management
- Contractor of Record
- PEO
- HRIS
- Recruiting
- Benefits
- Employment
- HR
- Compliance
- Workforce
- MCP
- AI Agents
---
