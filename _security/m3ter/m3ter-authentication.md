---
api_key_in: []
api_specs:
- filename: m3ter-openapi.yml
  format: yaml
  label: M3ter API
  slug: m3ter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/m3ter/refs/heads/main/openapi/m3ter-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: M3Ter Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: M3ter secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: M3ter
provider_slug: m3ter
scheme_count: 1
schemes:
- description: 'm3ter supports machine to machine authentication using the `clientCredentials` OAuth2 flow.


    The `authorizationCode` flow controls access for human users via the m3ter Console application.'
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: /oauth/token
  - authorizationUrl: https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/m3ter-openapi.yml
  type: oauth2
slug: m3ter-authentication
source_filename: m3ter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/m3ter-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 4\n  - flow: authorizationCode\n    authorizationUrl: https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/token\n    scopes: 6\n  description: |-\n    m3ter supports machine to machine authentication using the `clientCredentials` OAuth2 flow.\n\n    The `authorizationCode` flow controls access for human users via the m3ter Console application.\n  sources:\n  - openapi/m3ter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m3ter/refs/heads/main/authentication/m3ter-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- FinOps
- Usage-Based Billing
- Metering
- Billing
- Pricing
- SaaS
---
