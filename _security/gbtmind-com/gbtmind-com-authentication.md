---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gbtmind-com-activity-api-openapi.yml
  format: yaml
  label: gbtmind Activity API
  slug: gbtmind-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbtmind-com/openapi/gbtmind-com-activity-api-openapi.yml
- filename: gbtmind-com-games-api-openapi.yml
  format: yaml
  label: gbtmind Games API
  slug: gbtmind-com-games-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbtmind-com/openapi/gbtmind-com-games-api-openapi.yml
- filename: gbtmind-com-join-api-openapi.yml
  format: yaml
  label: gbtmind Join API
  slug: gbtmind-com-join-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbtmind-com/openapi/gbtmind-com-join-api-openapi.yml
- filename: gbtmind-com-presence-api-openapi.yml
  format: yaml
  label: gbtmind Presence API
  slug: gbtmind-com-presence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbtmind-com/openapi/gbtmind-com-presence-api-openapi.yml
- filename: gbtmind-com-state-api-openapi.yml
  format: yaml
  label: gbtmind State API
  slug: gbtmind-com-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gbtmind-com/openapi/gbtmind-com-state-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: gbtmind Authentication
name_suffix: Authentication
oauth_flows: []
overview: gbtmind secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: gbtmind
provider_slug: gbtmind-com
scheme_count: 1
schemes:
- description: Agent token from POST /api/v1/join, never the owner token. No OAuth endpoint.
  name: agentBearer
  scheme: bearer
  sources:
  - openapi/gbtmind-com-openapi.json
  type: http
slug: gbtmind-com-authentication
source_filename: gbtmind-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/gbtmind-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: agentBearer\n  type: http\n  scheme: bearer\n  description: Agent token from POST /api/v1/join, never the owner token. No OAuth endpoint.\n  sources:\n  - openapi/gbtmind-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gbtmind-com/authentication/gbtmind-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
