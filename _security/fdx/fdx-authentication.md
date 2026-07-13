---
api_key_in: []
api_specs:
- filename: core-exchange
  format: yaml
  label: FDX Accounts API
  slug: fdx-accounts-api
  spec_type: OpenAPI
  url: https://github.com/plaid/core-exchange
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Fdx Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Financial Data Exchange (FDX) secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Financial Data Exchange (FDX)
provider_slug: fdx
scheme_count: 2
schemes:
- description: 'This API uses an [OpenID Connect (OIDC) authentication flow](/core-exchange/authentication) and accepts the resulting [access token](/core-exchange/authentication#response-parameters) as a bearer token. For example,  `curl -H ''Authorization: Bearer <ACCESS&#95;TOKEN|''`.'
  name: openIdConnect
  openIdConnectUrl: https://www.your-organization.com/.well-known/openid-configuration
  sources:
  - openapi/fdx-corex-6.0.0.yaml
  - openapi/fdx-corex-6.2.0.yaml
  - openapi/fdx-corex-6.3.1.yaml
  type: openIdConnect
- description: 'This API uses an [OAuth2.0 authorization code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow) and accepts the resulting access token as a bearer token. For example,  `curl -H ''Authorization: Bearer <ACCESS&#95;TOKEN|''`.'
  flows:
  - authorizationUrl: https://www.your-organization.com/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://www.your-organization.com/token
  name: oauth2
  sources:
  - openapi/fdx-corex-6.0.0.yaml
  - openapi/fdx-corex-6.2.0.yaml
  - openapi/fdx-corex-6.3.1.yaml
  type: oauth2
slug: fdx-authentication
source_filename: fdx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fdx-corex-6.0.0.yaml, openapi/fdx-corex-6.2.0.yaml, openapi/fdx-corex-6.3.1.yaml\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.your-organization.com/.well-known/openid-configuration\n  description: 'This API uses an [OpenID Connect (OIDC) authentication flow](/core-exchange/authentication)\n    and accepts the resulting [access token](/core-exchange/authentication#response-parameters)\n    as a bearer token. For example,  `curl -H ''Authorization: Bearer <ACCESS&#95;TOKEN|''`.'\n  sources:\n  - openapi/fdx-corex-6.0.0.yaml\n  - openapi/fdx-corex-6.2.0.yaml\n  - openapi/fdx-corex-6.3.1.yaml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.your-organization.com/authorize\n    tokenUrl: https://www.your-organization.com/token\n    scopes:\
  \ 3\n  description: 'This API uses an [OAuth2.0 authorization code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow)\n    and accepts the resulting access token as a bearer token. For example,  `curl -H ''Authorization:\n    Bearer <ACCESS&#95;TOKEN|''`.'\n  sources:\n  - openapi/fdx-corex-6.0.0.yaml\n  - openapi/fdx-corex-6.2.0.yaml\n  - openapi/fdx-corex-6.3.1.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/authentication/fdx-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Financial Data
- Open Banking
- Open Finance
- Financial Data Exchange
- Consumer Permissioned
- Account Data
- Transactions
- Investments
- Insurance
- Tax Data
- Payroll
- REST
- OAuth2
- FAPI
- CFPB 1033
---
