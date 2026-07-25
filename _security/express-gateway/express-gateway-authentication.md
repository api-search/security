---
api_key_in:
- header
api_specs:
- filename: express-gateway-apps-api-openapi.yml
  format: yaml
  label: Express Gateway Apps API
  slug: express-gateway-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-apps-api-openapi.yml
- filename: express-gateway-credentials-api-openapi.yml
  format: yaml
  label: Express Gateway Credentials API
  slug: express-gateway-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-credentials-api-openapi.yml
- filename: express-gateway-scopes-api-openapi.yml
  format: yaml
  label: Express Gateway Scopes API
  slug: express-gateway-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-scopes-api-openapi.yml
- filename: express-gateway-users-api-openapi.yml
  format: yaml
  label: Express Gateway Users API
  slug: express-gateway-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Express Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Express Gateway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Express Gateway
provider_slug: express-gateway
scheme_count: 1
schemes:
- description: 'When the Admin API is fronted by Express Gateway with key-auth,

    send "Authorization: apikey {keyId}:{keySecret}".'
  in: header
  name: KeyAuth
  parameter: Authorization
  sources:
  - openapi/express-gateway-openapi.yml
  type: apiKey
slug: express-gateway-authentication
source_filename: express-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/express-gateway-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: KeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    When the Admin API is fronted by Express Gateway with key-auth,\n    send \"Authorization: apikey {keyId}:{keySecret}\".\n  sources:\n  - openapi/express-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/authentication/express-gateway-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Composition
- API Gateway
- BFF
---
