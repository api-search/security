---
api_key_in: []
api_specs:
- filename: infor-ion-api-gateway-openapi.yml
  format: yaml
  label: Infor ION API Gateway
  slug: infor-ion-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/openapi/infor-ion-api-gateway-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Infor Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Infor secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Infor
provider_slug: infor
scheme_count: 2
schemes:
- description: Infor ION API Client Credentials grant
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2
  name: OAuth2ClientCredentials
  sources:
  - openapi/infor-ion-api-gateway-openapi.yml
  type: oauth2
- description: Infor ION API Authorization Code grant
  flows:
  - authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2
  name: OAuth2AuthorizationCode
  sources:
  - openapi/infor-ion-api-gateway-openapi.yml
  type: oauth2
slug: infor-authentication
source_filename: infor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/infor-ion-api-gateway-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n    scopes: 0\n  description: Infor ION API Client Credentials grant\n  sources:\n  - openapi/infor-ion-api-gateway-openapi.yml\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://inforos.infor.com/INFOR_DEV/as/authorization.oauth2\n    tokenUrl: https://inforos.infor.com/INFOR_DEV/as/token.oauth2\n    scopes: 0\n  description: Infor ION API Authorization Code grant\n  sources:\n  - openapi/infor-ion-api-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infor/refs/heads/main/authentication/infor-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- ERP
- Manufacturing
- Supply Chain
- Cloud
- Integration
---
