---
api_key_in: []
api_specs:
- filename: porter-bundle-openapi.yml
  format: yaml
  label: Porter Bundle API
  slug: porter-bundle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/porter/refs/heads/main/openapi/porter-bundle-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Porter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Porter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Porter
provider_slug: porter
scheme_count: 1
schemes:
- description: Bearer token for authenticating to the Porter server API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/porter-bundle-openapi.yml
  type: http
slug: porter-authentication
source_filename: porter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/porter-bundle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for authenticating to the Porter server API.\n  sources:\n  - openapi/porter-bundle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/porter/refs/heads/main/authentication/porter-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Native
- CNAB
- DevOps
- Kubernetes
- Package Manager
---
