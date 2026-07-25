---
api_key_in: []
api_specs:
- filename: codecombat-auth-api-openapi.yml
  format: yaml
  label: CodeCombat Auth API
  slug: codecombat-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codecombat/refs/heads/main/openapi/codecombat-auth-api-openapi.yml
- filename: codecombat-clans-api-openapi.yml
  format: yaml
  label: CodeCombat Clans API
  slug: codecombat-clans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codecombat/refs/heads/main/openapi/codecombat-clans-api-openapi.yml
- filename: codecombat-classrooms-api-openapi.yml
  format: yaml
  label: CodeCombat Classrooms API
  slug: codecombat-classrooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codecombat/refs/heads/main/openapi/codecombat-classrooms-api-openapi.yml
- filename: codecombat-default-api-openapi.yml
  format: yaml
  label: CodeCombat Default API
  slug: codecombat-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codecombat/refs/heads/main/openapi/codecombat-default-api-openapi.yml
- filename: codecombat-stats-api-openapi.yml
  format: yaml
  label: CodeCombat Stats API
  slug: codecombat-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codecombat/refs/heads/main/openapi/codecombat-stats-api-openapi.yml
- filename: codecombat-users-api-openapi.yml
  format: yaml
  label: CodeCombat Users API
  slug: codecombat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codecombat/refs/heads/main/openapi/codecombat-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Codecombat Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeCombat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CodeCombat
provider_slug: codecombat
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/codecombat-openapi-original.yml
  type: http
slug: codecombat-authentication
source_filename: codecombat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/codecombat-openapi-original.yml\ndocs: https://api-docs.codecombat.com/\nnotes: >-\n  The CodeCombat Partner API authorizes every operation with HTTP Basic\n  authentication using a partner API key pair. OAuth2 in this API is a feature\n  for linking third-party SSO identities to users (add-oauth-identity /\n  login-oauth), not the API's own authorization mechanism.\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/codecombat-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codecombat/refs/heads/main/authentication/codecombat-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Education
- EdTech
- Coding
- Learning
- Classroom
- Students
- Gamification
- SSO
- Developer Tools
---
