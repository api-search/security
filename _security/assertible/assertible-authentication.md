---
api_key_in: []
api_specs:
- filename: assertible-openapi.yml
  format: yaml
  label: Assertible API
  slug: assertible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assertible/refs/heads/main/openapi/assertible-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Assertible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Assertible secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Assertible
provider_slug: assertible
scheme_count: 1
schemes:
- description: 'HTTP Basic auth where the username is the Assertible API token

    (`ASSERTIBLE_API_TOKEN`) and the password is left empty.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/assertible-openapi.yml
  type: http
slug: assertible-authentication
source_filename: assertible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/assertible-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth where the username is the Assertible API token\n    (`ASSERTIBLE_API_TOKEN`) and the password is left empty.\n  sources:\n  - openapi/assertible-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assertible/refs/heads/main/authentication/assertible-authentication.yml
summary_line: http · 1 scheme
tags:
- API Testing
- Monitoring
- Quality Assurance
- Testing
- CI/CD
---
