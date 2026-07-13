---
api_key_in: []
api_specs:
- filename: tooljet-tooljet-external-api-openapi.yml
  format: yaml
  label: ToolJet External API
  slug: tooljet-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooljet/refs/heads/main/openapi/tooljet-tooljet-external-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tooljet Authentication
name_suffix: Authentication
oauth_flows: []
overview: ToolJet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ToolJet
provider_slug: tooljet
scheme_count: 1
schemes:
- description: Static access token configured via the TOOLJET_SERVICE_TOKEN environment variable. Pass the token as the username with an empty password, encoded as Base64 in the Authorization header.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/tooljet-tooljet-external-api-openapi.yml
  type: http
slug: tooljet-authentication
source_filename: tooljet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tooljet-tooljet-external-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Static access token configured via the TOOLJET_SERVICE_TOKEN environment variable.\n    Pass the token as the username with an empty password, encoded as Base64 in the Authorization\n    header.\n  sources:\n  - openapi/tooljet-tooljet-external-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tooljet/refs/heads/main/authentication/tooljet-authentication.yml
summary_line: http · 1 scheme
tags:
- low-code
- internal tools
- open-source
- application builder
- workflow automation
- no-code
- dashboards
- AI agents
---
