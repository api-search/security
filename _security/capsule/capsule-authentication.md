---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Capsule REST API
  slug: capsule-rest-api
  spec_type: OpenAPI
  url: https://developer.capsulecrm.com/
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Capsule Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capsule secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Capsule
provider_slug: capsule
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'OAuth 2.0 access token or personal access token. The OAuth

    authorization endpoint is https://api.capsulecrm.com/oauth/authorise

    and the token endpoint is https://api.capsulecrm.com/oauth/token.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/capsule-openapi.yml
  type: http
slug: capsule-authentication
source_filename: capsule-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/capsule-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    OAuth 2.0 access token or personal access token. The OAuth\n    authorization endpoint is https://api.capsulecrm.com/oauth/authorise\n    and the token endpoint is https://api.capsulecrm.com/oauth/token.\n  sources:\n  - openapi/capsule-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/authentication/capsule-authentication.yml
summary_line: http · 1 scheme
tags:
- Contact Management
- CRM
- Custom Fields
- Opportunities
- Pipelines
- Project Management
- REST
- Sales
- Tasks
- Webhooks
---
