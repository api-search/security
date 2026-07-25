---
api_key_in: []
api_specs:
- filename: ambassador-diagnostics-api-openapi.yml
  format: yaml
  label: Ambassador Diagnostics API
  slug: ambassador-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-diagnostics-api-openapi.yml
- filename: ambassador-hosts-api-openapi.yml
  format: yaml
  label: Ambassador Hosts API
  slug: ambassador-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-hosts-api-openapi.yml
- filename: ambassador-mappings-api-openapi.yml
  format: yaml
  label: Ambassador Mappings API
  slug: ambassador-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-mappings-api-openapi.yml
- filename: ambassador-modules-api-openapi.yml
  format: yaml
  label: Ambassador Modules API
  slug: ambassador-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-modules-api-openapi.yml
- filename: ambassador-ratelimits-api-openapi.yml
  format: yaml
  label: Ambassador RateLimits API
  slug: ambassador-ratelimits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-ratelimits-api-openapi.yml
- filename: ambassador-tlscontexts-api-openapi.yml
  format: yaml
  label: Ambassador TLSContexts API
  slug: ambassador-tlscontexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/openapi/ambassador-tlscontexts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ambassador Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ambassador secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ambassador
provider_slug: ambassador
scheme_count: 1
schemes:
- description: Bearer token authentication. Tokens are managed through the Ambassador Edge Stack management interface or Kubernetes service account tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ambassador-openapi.yml
  type: http
slug: ambassador-authentication
source_filename: ambassador-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ambassador-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Tokens are managed through the Ambassador Edge Stack\n    management interface or Kubernetes service account tokens.\n  sources:\n  - openapi/ambassador-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/authentication/ambassador-authentication.yml
summary_line: http · 1 scheme
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
---
