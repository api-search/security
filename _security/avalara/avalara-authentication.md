---
api_key_in: []
api_specs:
- filename: avalara-avatax-rest-openapi.yml
  format: yaml
  label: AvaTax APIs
  slug: avatax-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-avatax-rest-openapi.yml
- filename: avalara-communications-openapi.yml
  format: yaml
  label: Communications Tax API
  slug: communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-communications-openapi.yml
- filename: avalara-excise-openapi.yml
  format: yaml
  label: Excise Platform API
  slug: excise-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-excise-openapi.yml
- filename: avalara-item-classification-openapi.yml
  format: yaml
  label: Item Classification API
  slug: item-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-item-classification-openapi.yml
- filename: avalara-avatax-brazil-openapi.yml
  format: yaml
  label: AvaTax Brazil API
  slug: avatax-brazil-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-avatax-brazil-openapi.yml
- filename: avalara-vat-reporting-openapi.yml
  format: yaml
  label: VAT Reporting API
  slug: vat-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-vat-reporting-openapi.yml
- filename: avalara-mylodgetax-openapi.yml
  format: yaml
  label: MyLodgeTax API
  slug: mylodgetax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-mylodgetax-openapi.yml
- filename: avalara-certcapture-openapi.yml
  format: yaml
  label: CertCapture API
  slug: certcapture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-certcapture-openapi.yml
- filename: avalara-e-invoicing-openapi.yml
  format: yaml
  label: E-Invoicing REST API
  slug: e-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-e-invoicing-openapi.yml
- filename: avalara-activation-service-openapi.yml
  format: yaml
  label: Activation Service API
  slug: activation-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-activation-service-openapi.yml
- filename: avalara-business-openapi.yml
  format: yaml
  label: Avalara Business API
  slug: business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-business-openapi.yml
- filename: avalara-portal-oauth-openapi.yml
  format: yaml
  label: Portal OAuth API
  slug: portal-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-portal-oauth-openapi.yml
- filename: avalara-shared-company-service-openapi.yml
  format: yaml
  label: Shared Company Service API
  slug: shared-company-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-shared-company-service-openapi.yml
- filename: avalara-hs-code-classification-openapi.yml
  format: yaml
  label: Automated Tariff Code Classification API
  slug: hs-code-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-hs-code-classification-openapi.yml
- filename: avalara-1099-w9-openapi.yml
  format: yaml
  label: 1099 & W-9 API
  slug: 1099-w9-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-1099-w9-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Avalara Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
- deviceCode
- refreshToken
overview: Avalara secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, password, deviceCode, and refreshToken flow(s).
provider_name: Avalara
provider_slug: avalara
scheme_count: 3
schemes:
- description: OAuth 2.0 bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/avalara-1099-w9-openapi.yml
  - openapi/avalara-activation-service-openapi.yml
  - openapi/avalara-avatax-brazil-openapi.yml
  - openapi/avalara-avatax-rest-openapi.yml
  - openapi/avalara-business-openapi.yml
  - openapi/avalara-e-invoicing-openapi.yml
  - openapi/avalara-excise-openapi.yml
  - openapi/avalara-hs-code-classification-openapi.yml
  - openapi/avalara-item-classification-openapi.yml
  - openapi/avalara-mylodgetax-openapi.yml
  - openapi/avalara-shared-company-service-openapi.yml
  - openapi/avalara-vat-reporting-openapi.yml
  type: http
- description: Use your AvaTax username/password or accountId/licenseKey as basic auth credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/avalara-avatax-rest-openapi.yml
  - openapi/avalara-certcapture-openapi.yml
  - openapi/avalara-communications-openapi.yml
  - openapi/avatax-apis-openapi.yml
  type: http
- description: OAuth 2.0 / OpenID Connect via Avalara IdentityServer (identity.avalara.com). Supports authorization_code (+ PKCE S256), client_credentials, password, device_code, token-exchange and refresh_token grants.
  flows:
  - flow: clientCredentials
    tokenUrl: https://identity.avalara.com/connect/token
  - authorizationUrl: https://identity.avalara.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.avalara.com/connect/token
  name: AvalaraIdentity
  scopes_ref: scopes/avalara-scopes.yml
  source: https://identity.avalara.com/.well-known/openid-configuration
  type: oauth2
slug: avalara-authentication
source_filename: avalara-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/ security schemes + https://identity.avalara.com/.well-known/openid-configuration\ndocs: https://developer.avalara.com/avatax/authentication-in-rest/\nnotes: >-\n  The per-API OpenAPI specs declare HTTP basic and bearer schemes. AvaTax REST v2\n  accepts either HTTP basic (username/password, or accountId/licenseKey) or an\n  OAuth 2.0 bearer token. Platform authorization is OAuth 2.0 / OIDC issued by\n  IdentityServer at identity.avalara.com (see scopes/avalara-scopes.yml for the\n  full endpoint + scope surface). Upgraded from derived to searched with the docs\n  auth page and the live OIDC discovery document.\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes: [basic, bearer]\n  oauth2_flows: [authorizationCode, clientCredentials, password, deviceCode, refreshToken]\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token\n  sources:\n  - openapi/avalara-1099-w9-openapi.yml\n\
  \  - openapi/avalara-activation-service-openapi.yml\n  - openapi/avalara-avatax-brazil-openapi.yml\n  - openapi/avalara-avatax-rest-openapi.yml\n  - openapi/avalara-business-openapi.yml\n  - openapi/avalara-e-invoicing-openapi.yml\n  - openapi/avalara-excise-openapi.yml\n  - openapi/avalara-hs-code-classification-openapi.yml\n  - openapi/avalara-item-classification-openapi.yml\n  - openapi/avalara-mylodgetax-openapi.yml\n  - openapi/avalara-shared-company-service-openapi.yml\n  - openapi/avalara-vat-reporting-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your AvaTax username/password or accountId/licenseKey as basic auth credentials\n  sources:\n  - openapi/avalara-avatax-rest-openapi.yml\n  - openapi/avalara-certcapture-openapi.yml\n  - openapi/avalara-communications-openapi.yml\n  - openapi/avatax-apis-openapi.yml\n- name: AvalaraIdentity\n  type: oauth2\n  description: >-\n    OAuth 2.0 / OpenID Connect via Avalara IdentityServer (identity.avalara.com).\n\
  \    Supports authorization_code (+ PKCE S256), client_credentials, password,\n    device_code, token-exchange and refresh_token grants.\n  source: https://identity.avalara.com/.well-known/openid-configuration\n  flows:\n    - flow: clientCredentials\n      tokenUrl: https://identity.avalara.com/connect/token\n    - flow: authorizationCode\n      authorizationUrl: https://identity.avalara.com/connect/authorize\n      tokenUrl: https://identity.avalara.com/connect/token\n  scopes_ref: scopes/avalara-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/authentication/avalara-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Taxes
---
