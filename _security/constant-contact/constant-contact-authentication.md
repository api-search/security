---
api_key_in:
- header
api_specs:
- filename: swagger.yaml
  format: yaml
  label: Constant Contact V3 API
  slug: v3
  spec_type: OpenAPI
  url: https://api.cc.email/v3/swagger.yaml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Constant Contact Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Constant Contact secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Constant Contact
provider_slug: constant-contact
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize
    flow: implicit
    scopes: 4
  name: oauth2_implicit
  sources:
  - openapi/constant-contact-v3-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://authz.constantcontact.com/oauth2/default/v1/token
  name: oauth2_access_code
  sources:
  - openapi/constant-contact-v3-openapi.yml
  type: oauth2
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/constant-contact-v3-openapi.yml
  type: apiKey
slug: constant-contact-authentication
source_filename: constant-contact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/constant-contact-v3-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: oauth2_implicit\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize\n    scopes: 4\n  sources:\n  - openapi/constant-contact-v3-openapi.yml\n- name: oauth2_access_code\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authz.constantcontact.com/oauth2/default/v1/authorize\n    tokenUrl: https://authz.constantcontact.com/oauth2/default/v1/token\n    scopes: 4\n  sources:\n  - openapi/constant-contact-v3-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/constant-contact-v3-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/authentication/constant-contact-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Campaigns
- Contacts
- Email Marketing
- Events
- Reporting
- SMS
- Surveys
---
