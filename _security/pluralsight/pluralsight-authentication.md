---
api_key_in: []
api_specs:
- filename: pluralsight-catalog-api-openapi.yml
  format: yaml
  label: Pluralsight Catalog API
  slug: pluralsight-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-catalog-api-openapi.yml
- filename: pluralsight-coding-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight Coding Metrics API
  slug: pluralsight-coding-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-coding-metrics-api-openapi.yml
- filename: pluralsight-collaboration-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight Collaboration Metrics API
  slug: pluralsight-collaboration-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-collaboration-metrics-api-openapi.yml
- filename: pluralsight-commits-api-openapi.yml
  format: yaml
  label: Pluralsight Commits API
  slug: pluralsight-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-commits-api-openapi.yml
- filename: pluralsight-dora-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight DORA Metrics API
  slug: pluralsight-dora-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-dora-metrics-api-openapi.yml
- filename: pluralsight-graphql-api-openapi.yml
  format: yaml
  label: Pluralsight GraphQL API
  slug: pluralsight-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-graphql-api-openapi.yml
- filename: pluralsight-integrations-api-openapi.yml
  format: yaml
  label: Pluralsight Integrations API
  slug: pluralsight-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-integrations-api-openapi.yml
- filename: pluralsight-licensing-api-openapi.yml
  format: yaml
  label: Pluralsight Licensing API
  slug: pluralsight-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-licensing-api-openapi.yml
- filename: pluralsight-pull-requests-api-openapi.yml
  format: yaml
  label: Pluralsight Pull Requests API
  slug: pluralsight-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-pull-requests-api-openapi.yml
- filename: pluralsight-reports-api-openapi.yml
  format: yaml
  label: Pluralsight Reports API
  slug: pluralsight-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-reports-api-openapi.yml
- filename: pluralsight-repos-api-openapi.yml
  format: yaml
  label: Pluralsight Repos API
  slug: pluralsight-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-repos-api-openapi.yml
- filename: pluralsight-teams-api-openapi.yml
  format: yaml
  label: Pluralsight Teams API
  slug: pluralsight-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-teams-api-openapi.yml
- filename: pluralsight-tickets-api-openapi.yml
  format: yaml
  label: Pluralsight Tickets API
  slug: pluralsight-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-tickets-api-openapi.yml
- filename: pluralsight-users-api-openapi.yml
  format: yaml
  label: Pluralsight Users API
  slug: pluralsight-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Pluralsight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pluralsight secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pluralsight
provider_slug: pluralsight
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pluralsight-coding-metrics-api-openapi.yml
  - openapi/pluralsight-collaboration-metrics-api-openapi.yml
  - openapi/pluralsight-commits-api-openapi.yml
  - openapi/pluralsight-dora-metrics-api-openapi.yml
  - openapi/pluralsight-graphql-api-openapi.yml
  - openapi/pluralsight-integrations-api-openapi.yml
  - openapi/pluralsight-licensing-api-openapi.yml
  - openapi/pluralsight-pull-requests-api-openapi.yml
  - openapi/pluralsight-reports-api-openapi.yml
  - openapi/pluralsight-repos-api-openapi.yml
  - openapi/pluralsight-teams-api-openapi.yml
  - openapi/pluralsight-tickets-api-openapi.yml
  - openapi/pluralsight-users-api-openapi.yml
  type: http
slug: pluralsight-authentication
source_filename: pluralsight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: openapi/pluralsight-coding-metrics-api-openapi.yml, openapi/pluralsight-collaboration-metrics-api-openapi.yml,\n  openapi/pluralsight-commits-api-openapi.yml, openapi/pluralsight-dora-metrics-api-openapi.yml,\n  openapi/pluralsight-graphql-api-openapi.yml, openapi/pluralsight-integrations-api-openapi.yml,\n  openapi/pluralsight-licensing-api-openapi.yml, openapi/pluralsight-pull-requests-api-openapi.yml,\n  openapi/pluralsight-reports-api-openapi.yml, openapi/pluralsight-repos-api-openapi.yml, openapi/pluralsight-teams-api-openapi.yml,\n  openapi/pluralsight-tickets-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/pluralsight-coding-metrics-api-openapi.yml\n  - openapi/pluralsight-collaboration-metrics-api-openapi.yml\n  - openapi/pluralsight-commits-api-openapi.yml\n  - openapi/pluralsight-dora-metrics-api-openapi.yml\n\
  \  - openapi/pluralsight-graphql-api-openapi.yml\n  - openapi/pluralsight-integrations-api-openapi.yml\n  - openapi/pluralsight-licensing-api-openapi.yml\n  - openapi/pluralsight-pull-requests-api-openapi.yml\n  - openapi/pluralsight-reports-api-openapi.yml\n  - openapi/pluralsight-repos-api-openapi.yml\n  - openapi/pluralsight-teams-api-openapi.yml\n  - openapi/pluralsight-tickets-api-openapi.yml\n  - openapi/pluralsight-users-api-openapi.yml\n\ndocs: https://developer.pluralsight.com/manage-keys\nsearched: '2026-08-29'\nsearchedSources:\n- https://developer.pluralsight.com/manage-keys\n- https://developer.pluralsight.com/plan-permissions\n- https://developer.pluralsight.com/docs/getting-started/faqs\n- https://developer.pluralsight.com/docs/getting-started/release-stages\n- https://mcp.pluralsight.com/.well-known/oauth-authorization-server\nprofiles:\n- surface: Skills GraphQL API\n  endpoint: https://paas-api.pluralsight.com/graphql\n  type: apiKey\n  transport: bearer credential in\
  \ the HTTP Authorization header\n  issuance: >-\n    A Pluralsight PLAN ADMIN mints the key on https://developer.pluralsight.com/manage-keys. A\n    non-admin cannot request one directly - they must ask a plan admin. Multiple keys per plan are\n    supported.\n  entitlement:\n  - >-\n      Plan level - whether the plan carries the API entitlement at all, visible on\n      https://developer.pluralsight.com/plan-permissions.\n  - >-\n      Key level - the release stage attached to the individual key (General Release / Beta / Alpha).\n      Beta is a self-serve toggle on the key; Alpha is by invitation from support@pluralsight.com.\n  scopes: []\n  scopes_note: >-\n    There are no scopes. A key carries whatever its plan carries; an agent cannot request a narrower\n    grant.\n  key_metadata:\n  - >-\n      Each key should carry an email address - that address is how Pluralsight sends deprecation\n      notices for operations the key is observed using.\n  unauthenticated_response: '401 {\"\
  error\":\"AuthenticationError: Invalid API Key\"}'\n  observed: '2026-08-29'\n- surface: MCP Gateway\n  endpoint: https://mcp.pluralsight.com/mcp\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  dynamic_client_registration: https://mcp.pluralsight.com/register\n  authorization_endpoint: https://mcp.pluralsight.com/authorize\n  token_endpoint: https://mcp.pluralsight.com/token\n  jwks_uri: https://mcp.pluralsight.com/.well-known/jwks.json\n  token_endpoint_auth_methods_supported:\n  - none\n  scopes:\n  - invoke:gateway\n  - author:gateway\n  - employee:gateway\n  - admin:gateway\n  challenge: >-\n    401 with WWW-Authenticate: Bearer error=\"invalid_token\",\n    resource_metadata=\"https://mcp.pluralsight.com/.well-known/oauth-protected-resource\"\n  observed: '2026-08-29'\n  see_also: ../scopes/pluralsight-scopes.yml\nnote: >-\n  The bearerAuth/JWT scheme recorded in schemes[] above is what the OpenAPIs in this repo declare.\n  In practice the Skills API credential is a plan-admin\
  \ API key presented as a bearer token, not a\n  JWT issued by an authorization server; the only true OAuth surface Pluralsight operates is the MCP\n  gateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/authentication/pluralsight-authentication.yml
summary_line: http · 1 scheme
tags:
- Courses
- Education
- Engineering Metrics
- Learning
- Skills Assessment
- Technology
- Video Training
---
