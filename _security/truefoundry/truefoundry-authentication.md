---
api_key_in: []
api_specs:
- filename: truefoundry-ai-gateway-openapi.yml
  format: yaml
  label: TrueFoundry AI Gateway API
  slug: truefoundry-ai-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-ai-gateway-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Truefoundry Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueFoundry secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrueFoundry
provider_slug: truefoundry
scheme_count: 1
schemes:
- description: TrueFoundry API key (JWT format)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/truefoundry-ai-gateway-openapi.yml
  type: http
slug: truefoundry-authentication
source_filename: truefoundry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truefoundry-ai-gateway-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: TrueFoundry API key (JWT format)\n  sources:\n  - openapi/truefoundry-ai-gateway-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/authentication/truefoundry-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Platform
- Enterprise AI
- Kubernetes
- LLM Gateway
- MLOps
---
