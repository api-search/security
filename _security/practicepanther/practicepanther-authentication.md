---
api_key_in: []
api_specs:
- filename: practicepanther-practicepanther-api-openapi.yml
  format: yaml
  label: PracticePanther API
  slug: practicepanther-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/practicepanther/refs/heads/main/openapi/practicepanther-practicepanther-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Practicepanther Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: PracticePanther secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: PracticePanther
provider_slug: practicepanther
scheme_count: 1
schemes:
- description: OAuth 2.0 - Authorization Code Grant
  flows:
  - authorizationUrl: /OAuth/Authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: /OAuth/Token
  name: oauth2
  sources:
  - openapi/practicepanther-practicepanther-api-openapi.yml
  type: oauth2
slug: practicepanther-authentication
source_filename: practicepanther-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/practicepanther-practicepanther-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /OAuth/Authorize\n    tokenUrl: /OAuth/Token\n    scopes: 1\n  description: OAuth 2.0 - Authorization Code Grant\n  sources:\n  - openapi/practicepanther-practicepanther-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/practicepanther/refs/heads/main/authentication/practicepanther-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Legal
- Law Practice Management
- Case Management
- Billing
- Trust Accounting
- Time Tracking
- Legal Tech
---
