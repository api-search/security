---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: intodns-ai-ai-api-openapi.yml
  format: yaml
  label: IntoDNS.ai AI API
  slug: intodns-ai-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-ai-api-openapi.yml
- filename: intodns-ai-dns-api-openapi.yml
  format: yaml
  label: IntoDNS.ai Dns API
  slug: intodns-ai-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-dns-api-openapi.yml
- filename: intodns-ai-email-api-openapi.yml
  format: yaml
  label: IntoDNS.ai Email API
  slug: intodns-ai-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-email-api-openapi.yml
- filename: intodns-ai-scan-api-openapi.yml
  format: yaml
  label: IntoDNS.ai Scan API
  slug: intodns-ai-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-scan-api-openapi.yml
- filename: intodns-ai-system-api-openapi.yml
  format: yaml
  label: IntoDNS.ai System API
  slug: intodns-ai-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-system-api-openapi.yml
- filename: intodns-ai-web-api-openapi.yml
  format: yaml
  label: IntoDNS.ai Web API
  slug: intodns-ai-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-web-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: IntoDNS.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: IntoDNS.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IntoDNS.ai
provider_slug: intodns-ai
scheme_count: 1
schemes:
- description: Auth.js JWT session established by signing in at https://intodns.ai/login. On HTTPS the cookie is HttpOnly, Secure, SameSite=Lax, Path=/. Local HTTP development uses authjs.session-token without Secure. Auth.js manages cookies and numbered chunks when needed. This is browser session authentication, not an API key or bearer token; do not construct tokens or share session cookies with AI assistants.
  in: cookie
  name: SessionCookie
  parameter: __Secure-authjs.session-token
  sources:
  - openapi/intodns-ai-openapi.json
  type: apiKey
slug: intodns-ai-authentication
source_filename: intodns-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/intodns-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: __Secure-authjs.session-token\n  description: Auth.js JWT session established by signing in at https://intodns.ai/login. On\n    HTTPS the cookie is HttpOnly, Secure, SameSite=Lax, Path=/. Local HTTP development uses\n    authjs.session-token without Secure. Auth.js manages cookies and numbered chunks when needed.\n    This is browser session authentication, not an API key or bearer token; do not construct\n    tokens or share session cookies with AI assistants.\n  sources:\n  - openapi/intodns-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/intodns-ai/authentication/intodns-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DNS
- Email Security
- Artificial Intelligence
---
