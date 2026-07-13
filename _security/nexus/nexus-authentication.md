---
api_key_in: []
api_specs:
- filename: nexus-openapi.yml
  format: yaml
  label: Nexus Repository Manager REST API
  slug: nexus-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexus/refs/heads/main/openapi/nexus-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nexus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nexus Repository Manager secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nexus Repository Manager
provider_slug: nexus
scheme_count: 2
schemes:
- description: HTTP Basic authentication with a Nexus user account.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/nexus-openapi.yml
  type: http
- description: 'Nexus user token authentication. Tokens can be generated

    per user when User Tokens are enabled on the instance.'
  name: userToken
  scheme: bearer
  sources:
  - openapi/nexus-openapi.yml
  type: http
slug: nexus-authentication
source_filename: nexus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nexus-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with a Nexus user account.\n  sources:\n  - openapi/nexus-openapi.yml\n- name: userToken\n  type: http\n  scheme: bearer\n  description: |-\n    Nexus user token authentication. Tokens can be generated\n    per user when User Tokens are enabled on the instance.\n  sources:\n  - openapi/nexus-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexus/refs/heads/main/authentication/nexus-authentication.yml
summary_line: http · 2 schemes
tags:
- Artifact Management
- DevOps
- Docker
- Maven
- Npm
- Package Management
- Repository Manager
- Software Supply Chain
---
