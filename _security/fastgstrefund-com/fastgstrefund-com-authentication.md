---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fastgstrefund-com-checklist-api-openapi.yml
  format: yaml
  label: Fast GST Refund Checklist API
  slug: fastgstrefund-com-checklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastgstrefund-com/openapi/fastgstrefund-com-checklist-api-openapi.yml
- filename: fastgstrefund-com-generator-files-api-openapi.yml
  format: yaml
  label: Fast GST Refund Generator Files API
  slug: fastgstrefund-com-generator-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastgstrefund-com/openapi/fastgstrefund-com-generator-files-api-openapi.yml
- filename: fastgstrefund-com-generators-api-openapi.yml
  format: yaml
  label: Fast GST Refund Generators API
  slug: fastgstrefund-com-generators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastgstrefund-com/openapi/fastgstrefund-com-generators-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fast GST Refund Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fast GST Refund secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fast GST Refund
provider_slug: fastgstrefund-com
scheme_count: 1
schemes:
- description: OAuth 2.1 authorization code with S256 PKCE. Clients register at /oauth/register. The person signs in with an emailed code. See /.well-known/oauth-authorization-server.
  flows:
  - authorizationUrl: https://fastgstrefund.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://fastgstrefund.com/oauth/token
  name: account
  sources:
  - openapi/fastgstrefund-com-openapi.json
  type: oauth2
slug: fastgstrefund-com-authentication
source_filename: fastgstrefund-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/fastgstrefund-com-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: account\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fastgstrefund.com/oauth/authorize\n    tokenUrl: https://fastgstrefund.com/oauth/token\n    scopes: 1\n  description: OAuth 2.1 authorization code with S256 PKCE. Clients register at /oauth/register.\n    The person signs in with an emailed code. See /.well-known/oauth-authorization-server.\n  sources:\n  - openapi/fastgstrefund-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fastgstrefund-com/authentication/fastgstrefund-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- GST
- Refund
- JSON
- Export
- India
---
