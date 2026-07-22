---
api_key_in:
- header
api_specs:
- filename: venminder-digital-comply-openapi-original.json
  format: json
  label: Venminder API
  slug: venminder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venminder-digital-comply/refs/heads/main/openapi/venminder-digital-comply-openapi-original.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Venminder Digital Comply Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Venminder (Digital Comply) secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Venminder (Digital Comply)
provider_slug: venminder-digital-comply
scheme_count: 2
schemes:
- description: Please insert access token with Bearer into field eg. Bearer eyJhbGciOiJSUzI1Ni and click authorize.
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/venminder-digital-comply-openapi-original.json
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes:
      venminderApi: Access to the Venminder API
    tokenUrl: https://login.venminder.com/connect/token
  name: OAuth2 client credentials (docs)
  sources:
  - https://developers.venminder.com/ Token page
  type: oauth2
slug: venminder-digital-comply-authentication
source_filename: venminder-digital-comply-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/venminder-digital-comply-openapi-original.json + https://developers.venminder.com/ (Getting\n  Started, Venminder Token pages)\ndocs: https://developers.venminder.com/318218fb2/p/325101-getting-started\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  transport: HTTPS with TLS 1.2 required\nnotes: 'Authentication is OAuth 2.0 / OpenID Connect bearer tokens using the client-credentials grant.\n  Customers create an API Key (Client ID + Client Secret + expiration) in the Venminder Admin Panel (requires\n  the API Key Manager role; the API feature itself must be enabled by Venminder). The token endpoint is\n  https://login.venminder.com/connect/token with scope venminderApi; the resulting access token is sent\n  as an Authorization: Bearer header to rsd.venminder.com. Access tokens expire and must be refreshed\n  by re-authenticating.'\ntoken_endpoint: https://login.venminder.com/connect/token\n\
  grant_type: client_credentials\nscope: venminderApi\nexample: curl -v -X POST -d \"grant_type=client_credentials&scope=venminderApi\" -u <api_key>:<client_secret>\n  https://login.venminder.com/connect/token\noidc_discovery: well-known/venminder-digital-comply-openid-configuration.json\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Please insert access token with Bearer into field eg. Bearer eyJhbGciOiJSUzI1Ni and click\n    authorize.\n  sources:\n  - openapi/venminder-digital-comply-openapi-original.json\n- name: OAuth2 client credentials (docs)\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.venminder.com/connect/token\n    scopes:\n      venminderApi: Access to the Venminder API\n  sources:\n  - https://developers.venminder.com/ Token page\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venminder-digital-comply/refs/heads/main/authentication/venminder-digital-comply-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Third-Party Risk Management
- Vendor Management
- Risk
- Compliance
- Contracts
- Financial Services
- Due Diligence
- SCIM
---
