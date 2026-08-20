---
api_key_in: []
api_specs:
- filename: gluu-discovery-api-openapi.yml
  format: yaml
  label: Gluu discovery API
  slug: gluu-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/openapi/gluu-discovery-api-openapi.yml
- filename: gluu-fido-api-openapi.yml
  format: yaml
  label: Gluu fido API
  slug: gluu-fido-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/openapi/gluu-fido-api-openapi.yml
- filename: gluu-groups-api-openapi.yml
  format: yaml
  label: Gluu groups API
  slug: gluu-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/openapi/gluu-groups-api-openapi.yml
- filename: gluu-users-api-openapi.yml
  format: yaml
  label: Gluu users API
  slug: gluu-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/openapi/gluu-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gluu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gluu secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gluu
provider_slug: gluu
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token with SCIM scopes
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gluu-openapi.yml
  type: http
slug: gluu-authentication
source_filename: gluu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gluu-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token with SCIM scopes\n  sources:\n  - openapi/gluu-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/authentication/gluu-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Management
- Authentication
- Authorization
- IAM
- Identities
- OpenID Connect
---
