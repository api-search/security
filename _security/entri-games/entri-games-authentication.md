---
anonymous_access: false
api_key_in: []
api_specs:
- filename: entri-games-bar-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Bar API
  slug: entri-games-bar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-bar-api-openapi.yml
- filename: entri-games-catalog-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Catalog API
  slug: entri-games-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-catalog-api-openapi.yml
- filename: entri-games-chats-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Chats API
  slug: entri-games-chats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-chats-api-openapi.yml
- filename: entri-games-companies-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Companies API
  slug: entri-games-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-companies-api-openapi.yml
- filename: entri-games-context-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Context API
  slug: entri-games-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-context-api-openapi.yml
- filename: entri-games-events-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Events API
  slug: entri-games-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-events-api-openapi.yml
- filename: entri-games-inbox-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Inbox API
  slug: entri-games-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-inbox-api-openapi.yml
- filename: entri-games-interview-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Interview API
  slug: entri-games-interview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-interview-api-openapi.yml
- filename: entri-games-leads-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Leads API
  slug: entri-games-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-leads-api-openapi.yml
- filename: entri-games-me-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Me API
  slug: entri-games-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-me-api-openapi.yml
- filename: entri-games-operations-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Operations API
  slug: entri-games-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-operations-api-openapi.yml
- filename: entri-games-people-api-openapi.yml
  format: yaml
  label: Геймдев Таверна People API
  slug: entri-games-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-people-api-openapi.yml
- filename: entri-games-profile-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Profile API
  slug: entri-games-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-profile-api-openapi.yml
- filename: entri-games-projects-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Projects API
  slug: entri-games-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-projects-api-openapi.yml
- filename: entri-games-quests-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Quests API
  slug: entri-games-quests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-quests-api-openapi.yml
- filename: entri-games-suggestions-api-openapi.yml
  format: yaml
  label: Геймдев Таверна Suggestions API
  slug: entri-games-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri-games/openapi/entri-games-suggestions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Геймдев Таверна Authentication
name_suffix: Authentication
oauth_flows: []
overview: Геймдев Таверна secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Геймдев Таверна
provider_slug: entri-games
scheme_count: 1
schemes:
- description: OAuth access token (resource …/api/agent/v1) or agent key.
  name: agentBearer
  scheme: bearer
  sources:
  - openapi/entri-games-openapi.json
  type: http
slug: entri-games-authentication
source_filename: entri-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/entri-games-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: agentBearer\n  type: http\n  scheme: bearer\n  description: OAuth access token (resource …/api/agent/v1) or agent key.\n  sources:\n  - openapi/entri-games-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/entri-games/authentication/entri-games-authentication.yml
summary_line: http · 1 scheme
tags:
- Game Development
- Platform
- Community
- AI Agents
- Russian
---
