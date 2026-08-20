---
api_key_in: []
api_specs:
- filename: http-toolkit-client-api-openapi.yml
  format: yaml
  label: HTTP Toolkit client API
  slug: http-toolkit-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/openapi/http-toolkit-client-api-openapi.yml
- filename: http-toolkit-config-api-openapi.yml
  format: yaml
  label: HTTP Toolkit config API
  slug: http-toolkit-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/openapi/http-toolkit-config-api-openapi.yml
- filename: http-toolkit-interceptors-api-openapi.yml
  format: yaml
  label: HTTP Toolkit interceptors API
  slug: http-toolkit-interceptors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/openapi/http-toolkit-interceptors-api-openapi.yml
- filename: http-toolkit-server-api-openapi.yml
  format: yaml
  label: HTTP Toolkit server API
  slug: http-toolkit-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/openapi/http-toolkit-server-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Http Toolkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: HTTP Toolkit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HTTP Toolkit
provider_slug: http-toolkit
scheme_count: 1
schemes:
- description: Token-based authentication using a server-generated bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/http-toolkit-server-api-openapi.yml
  type: http
slug: http-toolkit-authentication
source_filename: http-toolkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/http-toolkit-server-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Token-based authentication using a server-generated bearer token\n  sources:\n  - openapi/http-toolkit-server-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/http-toolkit/refs/heads/main/authentication/http-toolkit-authentication.yml
summary_line: http · 1 scheme
tags:
- HTTP
- HTTPS
- Debugging
- Proxy
- Interception
- Mocking
- Testing
- Developer Tools
- Open-Source
---
