---
api_key_in: []
api_specs:
- filename: silverpop-authentication-api-openapi.yml
  format: yaml
  label: Silverpop Authentication API
  slug: silverpop-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-authentication-api-openapi.yml
- filename: silverpop-campaigns-api-openapi.yml
  format: yaml
  label: Silverpop Campaigns API
  slug: silverpop-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-campaigns-api-openapi.yml
- filename: silverpop-contacts-api-openapi.yml
  format: yaml
  label: Silverpop Contacts API
  slug: silverpop-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-contacts-api-openapi.yml
- filename: silverpop-programs-api-openapi.yml
  format: yaml
  label: Silverpop Programs API
  slug: silverpop-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-programs-api-openapi.yml
- filename: silverpop-reports-api-openapi.yml
  format: yaml
  label: Silverpop Reports API
  slug: silverpop-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-reports-api-openapi.yml
- filename: silverpop-transactional-api-openapi.yml
  format: yaml
  label: Silverpop Transactional API
  slug: silverpop-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-transactional-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Silverpop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Silverpop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Silverpop
provider_slug: silverpop
scheme_count: 1
schemes:
- description: OAuth 2.0 access token. Obtain via POST /oauth/token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/silverpop-openapi.yml
  type: http
slug: silverpop-authentication
source_filename: silverpop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/silverpop-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token. Obtain via POST /oauth/token.\n  sources:\n  - openapi/silverpop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/authentication/silverpop-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Marketing
- Marketing Automation
- Campaign Management
- Digital Marketing
---
