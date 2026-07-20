---
api_key_in: []
api_specs:
- filename: langai-api-openapi.yml
  format: yaml
  label: Lang.ai API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/openapi/langai-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Langai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lang.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lang.ai
provider_slug: langai
scheme_count: 1
schemes:
- description: 'Authenticate your account by including your secret API token in every request as an Authorization: Bearer header. Create a new API token from the Settings section of your Lang.ai instance. Generating a new token invalidates previously issued ones.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/langai-api-openapi.yml
  type: http
slug: langai-authentication
source_filename: langai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/langai-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authenticate your account by including your secret API token in every request\n    as an Authorization: Bearer header. Create a new API token from the Settings section of\n    your Lang.ai instance. Generating a new token invalidates previously issued ones.'\n  sources:\n  - openapi/langai-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/authentication/langai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Conversation Intelligence
- Customer Support
- Text Classification
- Analytics
- Customer Experience
---
