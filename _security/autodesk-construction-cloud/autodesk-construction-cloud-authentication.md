---
api_key_in: []
api_specs:
- filename: acc-admin-openapi.yml
  format: yaml
  label: Autodesk Construction Cloud Admin API
  slug: acc-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/openapi/acc-admin-openapi.yml
- filename: acc-issues-openapi.yml
  format: yaml
  label: Autodesk Construction Cloud Issues API
  slug: acc-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/openapi/acc-issues-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Autodesk Construction Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Autodesk Construction Cloud secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Autodesk Construction Cloud
provider_slug: autodesk-construction-cloud
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: oauth2ThreeLegged
  sources:
  - openapi/acc-admin-openapi.yml
  - openapi/acc-issues-openapi.yml
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: oauth2TwoLegged
  sources:
  - openapi/acc-admin-openapi.yml
  type: oauth2
slug: autodesk-construction-cloud-authentication
source_filename: autodesk-construction-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acc-admin-openapi.yml, openapi/acc-issues-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2ThreeLegged\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n    scopes: 4\n  sources:\n  - openapi/acc-admin-openapi.yml\n  - openapi/acc-issues-openapi.yml\n- name: oauth2TwoLegged\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n    scopes: 2\n  sources:\n  - openapi/acc-admin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/authentication/autodesk-construction-cloud-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Construction
- BIM
- Project Management
- AEC
- CAD
- Architecture
- Engineering
- Field Management
---
