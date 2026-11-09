---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentbits-dev-health-api-openapi.yml
  format: yaml
  label: Agent Bits Health API
  slug: agentbits-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbits-dev/openapi/agentbits-dev-health-api-openapi.yml
- filename: agentbits-dev-tool-api-openapi.yml
  format: yaml
  label: Agent Bits Tool API
  slug: agentbits-dev-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbits-dev/openapi/agentbits-dev-tool-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agentbits Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Bits secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Agent Bits
provider_slug: agentbits-dev
scheme_count: 1
schemes:
- bearerFormat: abt_<base64url>
  description: Project membership credential for the shelved private workspace/teams product (docs/PRODUCT-DIRECTION.md). Scope is determined by the authenticated membership. Never send credentials in URLs.
  name: projectCredential
  scheme: bearer
  sources:
  - openapi/agentbits-dev-openapi.json
  type: http
slug: agentbits-dev-authentication
source_filename: agentbits-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agentbits-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: projectCredential\n  type: http\n  scheme: bearer\n  bearerFormat: abt_<base64url>\n  description: Project membership credential for the shelved private workspace/teams product\n    (docs/PRODUCT-DIRECTION.md). Scope is determined by the authenticated membership. Never\n    send credentials in URLs.\n  sources:\n  - openapi/agentbits-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agentbits-dev/authentication/agentbits-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Utilities
- Data
- Tools
- Machine-Readable
---
