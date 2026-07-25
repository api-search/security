---
api_key_in: []
api_specs:
- filename: clever-events-api-openapi.yml
  format: yaml
  label: Clever Events API
  slug: clever-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-events-api-openapi.yml
- filename: clever-assignments-api-openapi.yml
  format: yaml
  label: Clever Assignments API
  slug: clever-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-assignments-api-openapi.yml
- filename: clever-courses-api-openapi.yml
  format: yaml
  label: Clever Courses API
  slug: clever-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-courses-api-openapi.yml
- filename: clever-districts-api-openapi.yml
  format: yaml
  label: Clever Districts API
  slug: clever-districts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-districts-api-openapi.yml
- filename: clever-resources-api-openapi.yml
  format: yaml
  label: Clever Resources API
  slug: clever-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-resources-api-openapi.yml
- filename: clever-schools-api-openapi.yml
  format: yaml
  label: Clever Schools API
  slug: clever-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-schools-api-openapi.yml
- filename: clever-sections-api-openapi.yml
  format: yaml
  label: Clever Sections API
  slug: clever-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-sections-api-openapi.yml
- filename: clever-submissions-api-openapi.yml
  format: yaml
  label: Clever Submissions API
  slug: clever-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-submissions-api-openapi.yml
- filename: clever-terms-api-openapi.yml
  format: yaml
  label: Clever Terms API
  slug: clever-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-terms-api-openapi.yml
- filename: clever-users-api-openapi.yml
  format: yaml
  label: Clever Users API
  slug: clever-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-users-api-openapi.yml
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
