---
api_key_in: []
api_specs:
- filename: oauth-token-endpoint.yml
  format: yaml
  label: OAuth 2.0 Authorization Server API
  slug: oauth-2-authorization-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oauth/refs/heads/main/openapi/oauth-token-endpoint.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oauth Authentication
name_suffix: Authentication
oauth_flows: []
overview: OAuth secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OAuth
provider_slug: oauth
scheme_count: 1
schemes:
- description: HTTP Basic authentication using the client_id as username and client_secret as password, as defined in RFC 6749 Section 2.3.1.
  name: ClientBasicAuth
  scheme: basic
  sources:
  - openapi/oauth-token-endpoint.yml
  type: http
slug: oauth-authentication
source_filename: oauth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oauth-token-endpoint.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ClientBasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the client_id as username and client_secret as\n    password, as defined in RFC 6749 Section 2.3.1.\n  sources:\n  - openapi/oauth-token-endpoint.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oauth/refs/heads/main/authentication/oauth-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Control
- Authorization
- OAuth
- Security
- Tokens
---
