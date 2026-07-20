---
api_key_in: []
api_specs:
- filename: garner-openapi-original.json
  format: json
  label: Garner Health API
  slug: garner-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/garner/refs/heads/main/openapi/garner-openapi-original.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Garner Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Garner secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Garner
provider_slug: garner
scheme_count: 2
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request_content_type: application/x-www-form-urlencoded
  request_params:
  - client_id
  - client_secret
  - grant_type
  sources:
  - https://garnerhealth.redoc.ly
  token_lifetime_seconds: 900
  token_type: Bearer
  token_url: https://api.getgarner.com/oauth2/token
  type: oauth2
- bearerFormat: API_TOKEN
  description: 'Legacy JWT bearer token provided at account setup; sent as `Authorization: Bearer <token>`. This is the scheme declared in the OpenAPI.'
  name: ApiToken
  scheme: bearer
  sources:
  - openapi/garner-openapi-original.json
  type: http
slug: garner-authentication
source_filename: garner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/garner-openapi-original.json\ndocs: https://garnerhealth.redoc.ly\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Garner APIs authenticate with OAuth 2.0 client-credentials access tokens.\n    A client_id and client_secret issued at account setup are exchanged at the\n    token endpoint for a short-lived Bearer access token. A legacy JWT bearer\n    token (issued at account setup) is also supported for older integrations.\n    The OpenAPI declares a single `ApiToken` http-bearer scheme; the OAuth2\n    client-credentials exchange is documented in the API reference narrative.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.getgarner.com/oauth2/token\n  grant_type: client_credentials\n  token_type: Bearer\n  token_lifetime_seconds: 900\n  request_content_type: application/x-www-form-urlencoded\n  request_params:\n\
  \  - client_id\n  - client_secret\n  - grant_type\n  sources:\n  - https://garnerhealth.redoc.ly\n- name: ApiToken\n  type: http\n  scheme: bearer\n  bearerFormat: API_TOKEN\n  description: >-\n    Legacy JWT bearer token provided at account setup; sent as\n    `Authorization: Bearer <token>`. This is the scheme declared in the OpenAPI.\n  sources:\n  - openapi/garner-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/garner/refs/heads/main/authentication/garner-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Healthtech
- Healthcare
- Provider Data
- Care Navigation
- Health Insurance
- Claims Analytics
- Provider Search
- Doctor Quality
---
