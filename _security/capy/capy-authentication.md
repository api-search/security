---
anonymous_access: false
api_key_in: []
api_specs:
- filename: capy-automations-api-openapi.yml
  format: yaml
  label: Capy Automations API
  slug: capy-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-automations-api-openapi.yml
- filename: capy-projects-api-openapi.yml
  format: yaml
  label: Capy Projects API
  slug: capy-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-projects-api-openapi.yml
- filename: capy-tasks-api-openapi.yml
  format: yaml
  label: Capy Tasks API
  slug: capy-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-tasks-api-openapi.yml
- filename: capy-threads-api-openapi.yml
  format: yaml
  label: Capy Threads API
  slug: capy-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-threads-api-openapi.yml
- filename: capy-usage-api-openapi.yml
  format: yaml
  label: Capy Usage API
  slug: capy-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-usage-api-openapi.yml
- filename: capy-captains-api-openapi.yml
  format: yaml
  label: Capy Captains API
  slug: capy-captains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-captains-api-openapi.yml
- filename: capy-folders-api-openapi.yml
  format: yaml
  label: Capy Folders API
  slug: capy-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-folders-api-openapi.yml
- filename: capy-messages-api-openapi.yml
  format: yaml
  label: Capy Messages API
  slug: capy-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-messages-api-openapi.yml
- filename: capy-reviewfilters-api-openapi.yml
  format: yaml
  label: Capy Review Filters API
  slug: capy-reviewfilters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-reviewfilters-api-openapi.yml
- filename: capy-reviewrules-api-openapi.yml
  format: yaml
  label: Capy Review Rules API
  slug: capy-reviewrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-reviewrules-api-openapi.yml
- filename: capy-reviews-api-openapi.yml
  format: yaml
  label: Capy Reviews API
  slug: capy-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-reviews-api-openapi.yml
- filename: capy-streams-api-openapi.yml
  format: yaml
  label: Capy Streams API
  slug: capy-streams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-streams-api-openapi.yml
- filename: capy-subagents-api-openapi.yml
  format: yaml
  label: Capy Subagents API
  slug: capy-subagents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-subagents-api-openapi.yml
- filename: capy-users-api-openapi.yml
  format: yaml
  label: Capy Users API
  slug: capy-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Capy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Capy
provider_slug: capy
scheme_count: 1
schemes:
- description: API token (capy_xxxx). Generate at capy.ai/settings/tokens
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/capy-openapi-original.json
  token_prefix: capy_
  type: http
slug: capy-authentication
source_filename: capy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/capy-openapi-original.json\ndocs: https://docs.capy.ai/api-reference/overview\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_format: capy_xxxx\n  header: 'Authorization: Bearer [example key]'\n  token_management: https://capy.ai/settings/tokens\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API token (capy_xxxx). Generate at capy.ai/settings/tokens\n  token_prefix: capy_\n  sources:\n  - openapi/capy-openapi-original.json\nnotes:\n- Session identity tokens (verifySession / getThreadSessionToken) are a separate,\n  short-lived token issued per captain session and written inside the VM at\n  /etc/capy/session-token (mode 0600); they are not API auth credentials but let\n  code prove a request came from a genuine Capy session.\n"
source_yaml_url: https://artifacts.apis.io/capy/authentication/capy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Coding Agents
- Software Engineering
- Developer Tools
- Automation
- Code Review
- DevOps
---
