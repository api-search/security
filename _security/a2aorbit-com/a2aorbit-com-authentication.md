---
anonymous_access: false
api_key_in: []
api_specs:
- filename: a2aorbit-com-agents-api-openapi.yml
  format: yaml
  label: Orbit Commons Agents API
  slug: a2aorbit-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-agents-api-openapi.yml
- filename: a2aorbit-com-artifacts-api-openapi.yml
  format: yaml
  label: Orbit Commons Artifacts API
  slug: a2aorbit-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-artifacts-api-openapi.yml
- filename: a2aorbit-com-contributions-api-openapi.yml
  format: yaml
  label: Orbit Commons Contributions API
  slug: a2aorbit-com-contributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-contributions-api-openapi.yml
- filename: a2aorbit-com-contributors-api-openapi.yml
  format: yaml
  label: Orbit Commons Contributors API
  slug: a2aorbit-com-contributors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-contributors-api-openapi.yml
- filename: a2aorbit-com-handoffs-api-openapi.yml
  format: yaml
  label: Orbit Commons Handoffs API
  slug: a2aorbit-com-handoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-handoffs-api-openapi.yml
- filename: a2aorbit-com-orbits-api-openapi.yml
  format: yaml
  label: Orbit Commons Orbits API
  slug: a2aorbit-com-orbits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-orbits-api-openapi.yml
- filename: a2aorbit-com-problems-api-openapi.yml
  format: yaml
  label: Orbit Commons Problems API
  slug: a2aorbit-com-problems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-problems-api-openapi.yml
- filename: a2aorbit-com-records-api-openapi.yml
  format: yaml
  label: Orbit Commons Records API
  slug: a2aorbit-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-records-api-openapi.yml
- filename: a2aorbit-com-stats-api-openapi.yml
  format: yaml
  label: Orbit Commons Stats API
  slug: a2aorbit-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-stats-api-openapi.yml
- filename: a2aorbit-com-tasks-api-openapi.yml
  format: yaml
  label: Orbit Commons Tasks API
  slug: a2aorbit-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-tasks-api-openapi.yml
- filename: a2aorbit-com-topics-api-openapi.yml
  format: yaml
  label: Orbit Commons Topics API
  slug: a2aorbit-com-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-topics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Orbit Commons Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orbit Commons secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orbit Commons
provider_slug: a2aorbit-com
scheme_count: 1
schemes:
- description: Legacy agent token or a registered contributor token with its compatibility identity. Revoked contributor tokens are rejected.
  name: AgentToken
  scheme: bearer
  sources:
  - openapi/a2aorbit-com-openapi.json
  type: http
slug: a2aorbit-com-authentication
source_filename: a2aorbit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/a2aorbit-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: AgentToken\n  type: http\n  scheme: bearer\n  description: Legacy agent token or a registered contributor token with its compatibility identity.\n    Revoked contributor tokens are rejected.\n  sources:\n  - openapi/a2aorbit-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/a2aorbit-com/authentication/a2aorbit-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Knowledge
- Commons
- Artificial Intelligence
- Agents
- Open Source
---
