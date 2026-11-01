---
anonymous_access: false
api_key_in: []
api_specs:
- filename: riskmodels-app-13f-filers-api-openapi.yml
  format: yaml
  label: riskmodels-app 13F Filers API
  slug: riskmodels-app-13f-filers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-13f-filers-api-openapi.yml
- filename: riskmodels-app-account-api-openapi.yml
  format: yaml
  label: riskmodels-app Account API
  slug: riskmodels-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-account-api-openapi.yml
- filename: riskmodels-app-authentication-api-openapi.yml
  format: yaml
  label: riskmodels-app Authentication API
  slug: riskmodels-app-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-authentication-api-openapi.yml
- filename: riskmodels-app-billing-api-openapi.yml
  format: yaml
  label: riskmodels-app Billing API
  slug: riskmodels-app-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-billing-api-openapi.yml
- filename: riskmodels-app-compliance-api-openapi.yml
  format: yaml
  label: riskmodels-app Compliance API
  slug: riskmodels-app-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-compliance-api-openapi.yml
- filename: riskmodels-app-deprecated-api-openapi.yml
  format: yaml
  label: riskmodels-app Deprecated API
  slug: riskmodels-app-deprecated-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-deprecated-api-openapi.yml
- filename: riskmodels-app-discovery-api-openapi.yml
  format: yaml
  label: riskmodels-app Discovery API
  slug: riskmodels-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-discovery-api-openapi.yml
- filename: riskmodels-app-fundamentals-api-openapi.yml
  format: yaml
  label: riskmodels-app Fundamentals API
  slug: riskmodels-app-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-fundamentals-api-openapi.yml
- filename: riskmodels-app-funds-api-openapi.yml
  format: yaml
  label: riskmodels-app Funds API
  slug: riskmodels-app-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-funds-api-openapi.yml
- filename: riskmodels-app-funds-data-plane-api-openapi.yml
  format: yaml
  label: riskmodels-app Funds Data Plane API
  slug: riskmodels-app-funds-data-plane-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-funds-data-plane-api-openapi.yml
- filename: riskmodels-app-mcp-api-openapi.yml
  format: yaml
  label: riskmodels-app MCP API
  slug: riskmodels-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-mcp-api-openapi.yml
- filename: riskmodels-app-plaid-integration-api-openapi.yml
  format: yaml
  label: riskmodels-app Plaid Integration API
  slug: riskmodels-app-plaid-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-plaid-integration-api-openapi.yml
- filename: riskmodels-app-privacy-api-openapi.yml
  format: yaml
  label: riskmodels-app Privacy API
  slug: riskmodels-app-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-privacy-api-openapi.yml
- filename: riskmodels-app-risk-metrics-api-openapi.yml
  format: yaml
  label: riskmodels-app Risk Metrics API
  slug: riskmodels-app-risk-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-risk-metrics-api-openapi.yml
- filename: riskmodels-app-utility-api-openapi.yml
  format: yaml
  label: riskmodels-app Utility API
  slug: riskmodels-app-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-utility-api-openapi.yml
- filename: riskmodels-app-webhooks-api-openapi.yml
  format: yaml
  label: riskmodels-app Webhooks API
  slug: riskmodels-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/riskmodels-app/openapi/riskmodels-app-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Riskmodels App Authentication
name_suffix: Authentication
oauth_flows: []
overview: riskmodels-app declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: riskmodels-app
provider_slug: riskmodels-app
scheme_count: 2
schemes:
- description: All external API calls use a Bearer token in the Authorization header.
  scheme: bearer
  token_location: header
  token_name: Authorization
  type: http
- authorizationUrl: https://riskmodels.app/oauth/authorize
  description: OAuth 2.0 Authorization Code flow with PKCE for user consent.
  flow: authorizationCode
  pkce: true
  scopes: {}
  tokenUrl: https://riskmodels.app/oauth/token
  type: oauth2
slug: riskmodels-app-authentication
source_filename: riskmodels-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://riskmodels.app/docs/authentication\nschemes:\n  - type: http\n    scheme: bearer\n    description: All external API calls use a Bearer token in the Authorization header.\n    token_location: header\n    token_name: Authorization\n  - type: oauth2\n    flow: authorizationCode\n    pkce: true\n    authorizationUrl: https://riskmodels.app/oauth/authorize\n    tokenUrl: https://riskmodels.app/oauth/token\n    scopes: {}\n    description: OAuth 2.0 Authorization Code flow with PKCE for user consent."
source_yaml_url: https://artifacts.apis.io/riskmodels-app/authentication/riskmodels-app-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Risk
- Analytics
- API
- Equity
---
