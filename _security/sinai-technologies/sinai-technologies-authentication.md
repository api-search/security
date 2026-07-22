---
api_key_in: []
api_specs:
- filename: sinai-technologies-openapi-original.yml
  format: yaml
  label: SINAI API
  slug: sinai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinai-technologies/refs/heads/main/openapi/sinai-technologies-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sinai Technologies Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Sinai Technologies secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Sinai Technologies
provider_slug: sinai-technologies
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: https://auth.sinai.com/oauth2/token
  name: OAuth2ClientCredentialsProduction
  sources:
  - openapi/sinai-technologies-openapi-original.yml
  type: oauth2
- flows:
  - authorizationUrl: https://auth.sinai.com/oauth2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://auth.sinai.com/oauth2/token
  name: OAuth2AuthCodeProduction
  sources:
  - openapi/sinai-technologies-openapi-original.yml
  type: oauth2
slug: sinai-technologies-authentication
source_filename: sinai-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sinai-technologies-openapi-original.yml\ndocs: https://docs.sinai.com/reference/accessing-the-api\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nnotes: >-\n  The SINAI HTTP API uses OAuth 2.0. Client Credentials is the machine-to-machine\n  (M2M) flow: POST application/x-www-form-urlencoded to the token endpoint with\n  grant_type=client_credentials, client_id, client_secret and an optional\n  space-separated scope list; the response is a Bearer access_token with\n  expires_in (3600s). Authorization Code is the delegated-user flow (authorize ->\n  code -> token) and returns a refresh_token; it currently supports no scopes,\n  authorizing instead against the user's configured access within the SINAI\n  platform. Tokens are sent as `Authorization: Bearer <token>`. The SINAI\n  web platform (not the API) additionally supports SSO via SAML 2.0.\nschemes:\n- name: OAuth2ClientCredentialsProduction\n\
  \  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sinai.com/oauth2/token\n    scopes: 6\n  sources:\n  - openapi/sinai-technologies-openapi-original.yml\n- name: OAuth2AuthCodeProduction\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.sinai.com/oauth2/authorize\n    tokenUrl: https://auth.sinai.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/sinai-technologies-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinai-technologies/refs/heads/main/authentication/sinai-technologies-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Carbon Management
- Carbon Accounting
- Emissions
- Sustainability
- ESG
- Decarbonization
- Climate
---
