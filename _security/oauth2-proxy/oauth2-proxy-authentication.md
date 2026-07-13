---
api_key_in:
- cookie
api_specs:
- filename: oauth2-proxy-openapi.yml
  format: yaml
  label: Oauth2-Proxy
  slug: oauth2-proxy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oauth2-proxy/refs/heads/main/openapi/oauth2-proxy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Oauth2 Proxy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oauth2-Proxy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oauth2-Proxy
provider_slug: oauth2-proxy
scheme_count: 1
schemes:
- description: Session cookie established by the OAuth callback.
  in: cookie
  name: SessionCookie
  parameter: _oauth2_proxy
  sources:
  - openapi/oauth2-proxy-openapi.yml
  type: apiKey
slug: oauth2-proxy-authentication
source_filename: oauth2-proxy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oauth2-proxy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: _oauth2_proxy\n  description: Session cookie established by the OAuth callback.\n  sources:\n  - openapi/oauth2-proxy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oauth2-proxy/refs/heads/main/authentication/oauth2-proxy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Authentication Proxy
- Proxy
---
