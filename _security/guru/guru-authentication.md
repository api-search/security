---
api_key_in: []
api_specs:
- filename: guru-analytics-api-openapi.yml
  format: yaml
  label: Guru Analytics API
  slug: guru-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-analytics-api-openapi.yml
- filename: guru-announcements-api-openapi.yml
  format: yaml
  label: Guru Announcements API
  slug: guru-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-announcements-api-openapi.yml
- filename: guru-answers-api-openapi.yml
  format: yaml
  label: Guru Answers API
  slug: guru-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-answers-api-openapi.yml
- filename: guru-cardcomments-api-openapi.yml
  format: yaml
  label: Guru CardComments API
  slug: guru-cardcomments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-cardcomments-api-openapi.yml
- filename: guru-cards-api-openapi.yml
  format: yaml
  label: Guru Cards API
  slug: guru-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-cards-api-openapi.yml
- filename: guru-cardverifiers-api-openapi.yml
  format: yaml
  label: Guru CardVerifiers API
  slug: guru-cardverifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-cardverifiers-api-openapi.yml
- filename: guru-collections-api-openapi.yml
  format: yaml
  label: Guru Collections API
  slug: guru-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-collections-api-openapi.yml
- filename: guru-folders-api-openapi.yml
  format: yaml
  label: Guru Folders API
  slug: guru-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-folders-api-openapi.yml
- filename: guru-groups-api-openapi.yml
  format: yaml
  label: Guru Groups API
  slug: guru-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-groups-api-openapi.yml
- filename: guru-members-api-openapi.yml
  format: yaml
  label: Guru Members API
  slug: guru-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-members-api-openapi.yml
- filename: guru-people-api-openapi.yml
  format: yaml
  label: Guru People API
  slug: guru-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-people-api-openapi.yml
- filename: guru-search-api-openapi.yml
  format: yaml
  label: Guru Search API
  slug: guru-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-search-api-openapi.yml
- filename: guru-tags-api-openapi.yml
  format: yaml
  label: Guru Tags API
  slug: guru-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-tags-api-openapi.yml
- filename: guru-tasks-api-openapi.yml
  format: yaml
  label: Guru Tasks API
  slug: guru-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-tasks-api-openapi.yml
- filename: guru-templates-api-openapi.yml
  format: yaml
  label: Guru Templates API
  slug: guru-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-templates-api-openapi.yml
- filename: guru-ticketlinking-api-openapi.yml
  format: yaml
  label: Guru TicketLinking API
  slug: guru-ticketlinking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-ticketlinking-api-openapi.yml
- filename: guru-user-api-openapi.yml
  format: yaml
  label: Guru User API
  slug: guru-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/openapi/guru-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Guru Authentication
name_suffix: Authentication
oauth_flows: []
overview: Guru secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Guru
provider_slug: guru
scheme_count: 2
schemes:
- description: API token authentication via HTTP Basic.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/guru-openapi.yml
  type: http
- description: OAuth 2.0 bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/guru-openapi.yml
  type: http
slug: guru-authentication
source_filename: guru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guru-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API token authentication via HTTP Basic.\n  sources:\n  - openapi/guru-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token.\n  sources:\n  - openapi/guru-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guru/refs/heads/main/authentication/guru-authentication.yml
summary_line: http · 2 schemes
tags:
- Knowledge Management
- Enterprise Search
- AI Knowledge Base
- Internal Wiki
- Verified Knowledge
- Workplace Productivity
---
