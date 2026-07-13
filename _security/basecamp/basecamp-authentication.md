---
api_key_in: []
api_specs:
- filename: basecamp-api-openapi.yml
  format: yaml
  label: Basecamp API
  slug: basecamp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-api-openapi.yml
- filename: basecamp-webhooks-asyncapi.yml
  format: yaml
  label: Basecamp Webhooks
  slug: basecamp-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/asyncapi/basecamp-webhooks-asyncapi.yml
- filename: basecamp-oauth-openapi.yml
  format: yaml
  label: Basecamp OAuth
  slug: basecamp-oauth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-oauth-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Basecamp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basecamp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Basecamp
provider_slug: basecamp
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Bearer token obtained via the Basecamp authorization code flow at launchpad.37signals.com. Include as "Authorization: Bearer {token}" in all requests.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/basecamp-api-openapi.yml
  - openapi/basecamp-oauth-openapi.yml
  type: http
slug: basecamp-authentication
source_filename: basecamp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/basecamp-api-openapi.yml, openapi/basecamp-oauth-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 Bearer token obtained via the Basecamp authorization code flow at\n    launchpad.37signals.com. Include as \"Authorization: Bearer {token}\" in all requests.'\n  sources:\n  - openapi/basecamp-api-openapi.yml\n  - openapi/basecamp-oauth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/authentication/basecamp-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
---
