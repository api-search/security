---
api_key_in: []
api_specs:
- filename: autodesk-authentication-openapi.yml
  format: yaml
  label: Autodesk Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-authentication-openapi.yml
- filename: autodesk-data-management-openapi.yml
  format: yaml
  label: Autodesk Data Management API
  slug: data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-data-management-openapi.yml
- filename: autodesk-model-derivative-openapi.yml
  format: yaml
  label: Autodesk Model Derivative API
  slug: model-derivative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-model-derivative-openapi.yml
- filename: autodesk-design-automation-openapi.yml
  format: yaml
  label: Autodesk Design Automation API
  slug: design-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-design-automation-openapi.yml
- filename: autodesk-webhooks-openapi.yml
  format: yaml
  label: Autodesk Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-webhooks-openapi.yml
- filename: autodesk-reality-capture-openapi.yml
  format: yaml
  label: Autodesk Reality Capture API
  slug: reality-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-reality-capture-openapi.yml
- filename: autodesk-sustainability-data-openapi.yml
  format: yaml
  label: Autodesk Sustainability Data API
  slug: sustainability-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-sustainability-data-openapi.yml
- filename: autodesk-parameters-openapi.yml
  format: yaml
  label: Autodesk Parameters API
  slug: parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-parameters-openapi.yml
- filename: autodesk-tandem-data-openapi.yml
  format: yaml
  label: Autodesk Tandem Data API
  slug: tandem-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-tandem-data-openapi.yml
- filename: autodesk-flow-graph-engine-openapi.yml
  format: yaml
  label: Autodesk Flow Graph Engine API
  slug: flow-graph-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-flow-graph-engine-openapi.yml
- filename: autodesk-acc-account-admin-openapi.yml
  format: yaml
  label: Autodesk ACC Account Admin API
  slug: acc-account-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-acc-account-admin-openapi.yml
- filename: autodesk-bim360-openapi.yml
  format: yaml
  label: Autodesk BIM 360 API
  slug: bim-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-bim360-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Autodesk Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Autodesk secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Autodesk
provider_slug: autodesk
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2ThreeLegged
  sources:
  - openapi/autodesk-acc-account-admin-openapi.yml
  - openapi/autodesk-authentication-openapi.yml
  - openapi/autodesk-bim360-openapi.yml
  - openapi/autodesk-data-management-openapi.yml
  - openapi/autodesk-model-derivative-openapi.yml
  - openapi/autodesk-parameters-openapi.yml
  - openapi/autodesk-tandem-data-openapi.yml
  - openapi/autodesk-webhooks-openapi.yml
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 11
    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token
  name: OAuth2TwoLegged
  sources:
  - openapi/autodesk-authentication-openapi.yml
  - openapi/autodesk-data-management-openapi.yml
  - openapi/autodesk-design-automation-openapi.yml
  - openapi/autodesk-flow-graph-engine-openapi.yml
  - openapi/autodesk-model-derivative-openapi.yml
  - openapi/autodesk-reality-capture-openapi.yml
  - openapi/autodesk-sustainability-data-openapi.yml
  - openapi/autodesk-webhooks-openapi.yml
  type: oauth2
slug: autodesk-authentication
source_filename: autodesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/autodesk-acc-account-admin-openapi.yml, openapi/autodesk-authentication-openapi.yml,\n  openapi/autodesk-bim360-openapi.yml, openapi/autodesk-data-management-openapi.yml, openapi/autodesk-design-automation-openapi.yml,\n  openapi/autodesk-flow-graph-engine-openapi.yml, openapi/autodesk-model-derivative-openapi.yml,\n  openapi/autodesk-parameters-openapi.yml, openapi/autodesk-reality-capture-openapi.yml, openapi/autodesk-sustainability-data-openapi.yml,\n  openapi/autodesk-tandem-data-openapi.yml, openapi/autodesk-webhooks-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2ThreeLegged\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.api.autodesk.com/authentication/v2/authorize\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n    scopes: 2\n  sources:\n  - openapi/autodesk-acc-account-admin-openapi.yml\n\
  \  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-bim360-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n  - openapi/autodesk-model-derivative-openapi.yml\n  - openapi/autodesk-parameters-openapi.yml\n  - openapi/autodesk-tandem-data-openapi.yml\n  - openapi/autodesk-webhooks-openapi.yml\n- name: OAuth2TwoLegged\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.api.autodesk.com/authentication/v2/token\n    scopes: 11\n  sources:\n  - openapi/autodesk-authentication-openapi.yml\n  - openapi/autodesk-data-management-openapi.yml\n  - openapi/autodesk-design-automation-openapi.yml\n  - openapi/autodesk-flow-graph-engine-openapi.yml\n  - openapi/autodesk-model-derivative-openapi.yml\n  - openapi/autodesk-reality-capture-openapi.yml\n  - openapi/autodesk-sustainability-data-openapi.yml\n  - openapi/autodesk-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/authentication/autodesk-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Fortune 1000
- 3D Modeling
- Architecture
- BIM
- CAD
- Construction
- Design
- Digital Twins
- Engineering
- Manufacturing
- Media and Entertainment
- Sustainability
---
