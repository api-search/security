---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flowral-app-auth-api-openapi.yml
  format: yaml
  label: Flowral Auth API
  slug: flowral-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-auth-api-openapi.yml
- filename: flowral-app-brainstorms-api-openapi.yml
  format: yaml
  label: Flowral Brainstorms API
  slug: flowral-app-brainstorms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-brainstorms-api-openapi.yml
- filename: flowral-app-flows-api-openapi.yml
  format: yaml
  label: Flowral Flows API
  slug: flowral-app-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-flows-api-openapi.yml
- filename: flowral-app-notifications-api-openapi.yml
  format: yaml
  label: Flowral Notifications API
  slug: flowral-app-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-notifications-api-openapi.yml
- filename: flowral-app-search-api-openapi.yml
  format: yaml
  label: Flowral Search API
  slug: flowral-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-search-api-openapi.yml
- filename: flowral-app-tasks-api-openapi.yml
  format: yaml
  label: Flowral Tasks API
  slug: flowral-app-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-tasks-api-openapi.yml
- filename: flowral-app-team-api-openapi.yml
  format: yaml
  label: Flowral Team API
  slug: flowral-app-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-team-api-openapi.yml
- filename: flowral-app-templates-api-openapi.yml
  format: yaml
  label: Flowral Templates API
  slug: flowral-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-templates-api-openapi.yml
- filename: flowral-app-work-api-openapi.yml
  format: yaml
  label: Flowral Work API
  slug: flowral-app-work-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-work-api-openapi.yml
- filename: flowral-app-workspace-api-openapi.yml
  format: yaml
  label: Flowral Workspace API
  slug: flowral-app-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowral-app/openapi/flowral-app-workspace-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Flowral Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Flowral secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Flowral
provider_slug: flowral-app
scheme_count: 2
schemes:
- description: 'An API key from the app: `Authorization: Bearer fl_sk_live_…`.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/flowral-app-openapi.json
  type: http
- description: Client credentials, for anything long-lived.
  flows:
  - flow: clientCredentials
    scopes: 8
    tokenUrl: https://api.flowral.app/v1/oauth/token
  name: oauth2
  sources:
  - openapi/flowral-app-openapi.json
  type: oauth2
slug: flowral-app-authentication
source_filename: flowral-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/flowral-app-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'An API key from the app: `Authorization: Bearer fl_sk_live_…`.'\n  sources:\n  - openapi/flowral-app-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flowral.app/v1/oauth/token\n    scopes: 8\n  description: Client credentials, for anything long-lived.\n  sources:\n  - openapi/flowral-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flowral-app/authentication/flowral-app-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Project Management
- Software-as-a-Service
- Collaboration
- Agencies
- Team
---
