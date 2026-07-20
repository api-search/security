---
api_key_in: []
api_specs:
- filename: code-ocean-openapi.yml
  format: yaml
  label: Code Ocean API
  slug: code-ocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/code-ocean/refs/heads/main/openapi/code-ocean-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Code Ocean Authentication
name_suffix: Authentication
oauth_flows: []
overview: Code Ocean secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Code Ocean
provider_slug: code-ocean
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Provide your Code Ocean access token (prefix `cop_`) as the basic-auth username with an empty password, e.g. `-u "cop_xxxxxxxxxx:"`.
  name: accessToken
  scheme: basic
  sources:
  - openapi/code-ocean-openapi.yml
  type: http
slug: code-ocean-authentication
source_filename: code-ocean-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/code-ocean-openapi.yml\ndocs: https://docs.codeocean.com/user-guide/code-ocean-api/authentication\nsummary:\n  types:\n  - http\n  token: scoped personal access token (prefix cop_), presented as HTTP Basic username with empty password\n  scopes_ref: scopes/code-ocean-scopes.yml\nschemes:\n- name: accessToken\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Provide your Code Ocean access token (prefix `cop_`)\n    as the basic-auth username with an empty password, e.g. `-u \"cop_xxxxxxxxxx:\"`.\n  sources:\n  - openapi/code-ocean-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code-ocean/refs/heads/main/authentication/code-ocean-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Reproducible Research
- Computational Science
- Data Science
- Research Computing
- Life Sciences
- Pipelines
- MLOps
- Cloud Platform
- Developer Tools
---
