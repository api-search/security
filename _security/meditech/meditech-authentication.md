---
api_key_in: []
api_specs:
- filename: meditech-fhir-openapi.yml
  format: yaml
  label: Meditech Expanse FHIR API
  slug: meditech-expanse-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-fhir-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Meditech Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: meditech secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: meditech
provider_slug: meditech
scheme_count: 1
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://yourhospital.meditech.com/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://yourhospital.meditech.com/oauth/token
  name: SMART_OAuth2
  sources:
  - openapi/meditech-fhir-openapi.yml
  type: oauth2
slug: meditech-authentication
source_filename: meditech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meditech-fhir-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: SMART_OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://yourhospital.meditech.com/oauth/authorize\n    tokenUrl: https://yourhospital.meditech.com/oauth/token\n    scopes: 5\n  description: SMART on FHIR OAuth 2.0 authorization\n  sources:\n  - openapi/meditech-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/authentication/meditech-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
