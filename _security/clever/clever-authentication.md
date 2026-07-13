---
api_key_in: []
api_specs:
- filename: clever-data-api-openapi.yml
  format: yaml
  label: Clever Data API
  slug: clever-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-data-api-openapi.yml
- filename: clever-lms-connect-api-openapi.yml
  format: yaml
  label: Clever LMS Connect API
  slug: clever-lms-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-lms-connect-api-openapi.yml
- filename: clever-events-api-openapi.yml
  format: yaml
  label: Clever Events API
  slug: clever-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-events-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Clever Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Clever secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Clever
provider_slug: clever
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://clever.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://clever.com/oauth/tokens
  name: oauth
  sources:
  - openapi/clever-data-api-openapi.yml
  - openapi/clever-events-api-openapi.yml
  - openapi/clever-lms-connect-api-openapi.yml
  type: oauth2
slug: clever-authentication
source_filename: clever-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clever-data-api-openapi.yml, openapi/clever-events-api-openapi.yml, openapi/clever-lms-connect-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clever.com/oauth/authorize\n    tokenUrl: https://clever.com/oauth/tokens\n    scopes: 0\n  sources:\n  - openapi/clever-data-api-openapi.yml\n  - openapi/clever-events-api-openapi.yml\n  - openapi/clever-lms-connect-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/authentication/clever-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- K-12
- EdTech
- Single Sign-On
- Rostering
- Identity
- SSO
- Student Data
- LMS
- SIS
---
