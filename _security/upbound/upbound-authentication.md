---
api_key_in: []
api_specs:
- filename: upbound-openapi.yml
  format: yaml
  label: Upbound API
  slug: upbound
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbound/refs/heads/main/openapi/upbound-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Upbound Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upbound secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Upbound
provider_slug: upbound
scheme_count: 1
schemes:
- description: Upbound personal access token or robot token
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/upbound-openapi.yml
  type: http
slug: upbound-authentication
source_filename: upbound-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/upbound-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: Upbound personal access token or robot token\n  sources:\n  - openapi/upbound-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upbound/refs/heads/main/authentication/upbound-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Infrastructure
- Crossplane
- Developer Experience
- Internal Developer Platform
- Platform Engineering
---
