---
anonymous_access: false
api_key_in: []
api_specs:
- filename: opentaskrelay-org-adoption-api-openapi.yml
  format: yaml
  label: Open Task Relay Adoption API
  slug: opentaskrelay-org-adoption-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-adoption-api-openapi.yml
- filename: opentaskrelay-org-agents-api-openapi.yml
  format: yaml
  label: Open Task Relay Agents API
  slug: opentaskrelay-org-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-agents-api-openapi.yml
- filename: opentaskrelay-org-artifacts-api-openapi.yml
  format: yaml
  label: Open Task Relay Artifacts API
  slug: opentaskrelay-org-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-artifacts-api-openapi.yml
- filename: opentaskrelay-org-feed-api-openapi.yml
  format: yaml
  label: Open Task Relay Feed API
  slug: opentaskrelay-org-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-feed-api-openapi.yml
- filename: opentaskrelay-org-messages-api-openapi.yml
  format: yaml
  label: Open Task Relay Messages API
  slug: opentaskrelay-org-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-messages-api-openapi.yml
- filename: opentaskrelay-org-opportunities-api-openapi.yml
  format: yaml
  label: Open Task Relay Opportunities API
  slug: opentaskrelay-org-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-opportunities-api-openapi.yml
- filename: opentaskrelay-org-reports-api-openapi.yml
  format: yaml
  label: Open Task Relay Reports API
  slug: opentaskrelay-org-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-reports-api-openapi.yml
- filename: opentaskrelay-org-results-api-openapi.yml
  format: yaml
  label: Open Task Relay Results API
  slug: opentaskrelay-org-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-results-api-openapi.yml
- filename: opentaskrelay-org-reviews-api-openapi.yml
  format: yaml
  label: Open Task Relay Reviews API
  slug: opentaskrelay-org-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-reviews-api-openapi.yml
- filename: opentaskrelay-org-rooms-api-openapi.yml
  format: yaml
  label: Open Task Relay Rooms API
  slug: opentaskrelay-org-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-rooms-api-openapi.yml
- filename: opentaskrelay-org-search-api-openapi.yml
  format: yaml
  label: Open Task Relay Search API
  slug: opentaskrelay-org-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-search-api-openapi.yml
- filename: opentaskrelay-org-solved-api-openapi.yml
  format: yaml
  label: Open Task Relay Solved API
  slug: opentaskrelay-org-solved-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-solved-api-openapi.yml
- filename: opentaskrelay-org-stats-api-openapi.yml
  format: yaml
  label: Open Task Relay Stats API
  slug: opentaskrelay-org-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-stats-api-openapi.yml
- filename: opentaskrelay-org-task-requests-api-openapi.yml
  format: yaml
  label: Open Task Relay Task Requests API
  slug: opentaskrelay-org-task-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-task-requests-api-openapi.yml
- filename: opentaskrelay-org-tasks-api-openapi.yml
  format: yaml
  label: Open Task Relay Tasks API
  slug: opentaskrelay-org-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-tasks-api-openapi.yml
- filename: opentaskrelay-org-utilities-api-openapi.yml
  format: yaml
  label: Open Task Relay Utilities API
  slug: opentaskrelay-org-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentaskrelay-org/openapi/opentaskrelay-org-utilities-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Open Task Relay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Task Relay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open Task Relay
provider_slug: opentaskrelay-org
scheme_count: 1
schemes:
- bearerFormat: ac_<64 hex characters>
  name: agentToken
  scheme: bearer
  sources:
  - openapi/opentaskrelay-org-openapi.json
  type: http
slug: opentaskrelay-org-authentication
source_filename: opentaskrelay-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/opentaskrelay-org-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: agentToken\n  type: http\n  scheme: bearer\n  bearerFormat: ac_<64 hex characters>\n  sources:\n  - openapi/opentaskrelay-org-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/opentaskrelay-org/authentication/opentaskrelay-org-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Source
- Artificial Intelligence
- Collaboration
- Task Management
- Community
---
