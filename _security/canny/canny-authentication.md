---
api_key_in:
- header
- query
api_specs:
- filename: canny-autopilot-api-openapi.yml
  format: yaml
  label: Canny Autopilot API
  slug: canny-autopilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-autopilot-api-openapi.yml
- filename: canny-boards-api-openapi.yml
  format: yaml
  label: Canny Boards API
  slug: canny-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-boards-api-openapi.yml
- filename: canny-categories-api-openapi.yml
  format: yaml
  label: Canny Categories API
  slug: canny-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-categories-api-openapi.yml
- filename: canny-changelogentries-api-openapi.yml
  format: yaml
  label: Canny ChangelogEntries API
  slug: canny-changelogentries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-changelogentries-api-openapi.yml
- filename: canny-comments-api-openapi.yml
  format: yaml
  label: Canny Comments API
  slug: canny-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-comments-api-openapi.yml
- filename: canny-companies-api-openapi.yml
  format: yaml
  label: Canny Companies API
  slug: canny-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-companies-api-openapi.yml
- filename: canny-groups-api-openapi.yml
  format: yaml
  label: Canny Groups API
  slug: canny-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-groups-api-openapi.yml
- filename: canny-ideas-api-openapi.yml
  format: yaml
  label: Canny Ideas API
  slug: canny-ideas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-ideas-api-openapi.yml
- filename: canny-insights-api-openapi.yml
  format: yaml
  label: Canny Insights API
  slug: canny-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-insights-api-openapi.yml
- filename: canny-opportunities-api-openapi.yml
  format: yaml
  label: Canny Opportunities API
  slug: canny-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-opportunities-api-openapi.yml
- filename: canny-posts-api-openapi.yml
  format: yaml
  label: Canny Posts API
  slug: canny-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-posts-api-openapi.yml
- filename: canny-statuschanges-api-openapi.yml
  format: yaml
  label: Canny StatusChanges API
  slug: canny-statuschanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-statuschanges-api-openapi.yml
- filename: canny-tags-api-openapi.yml
  format: yaml
  label: Canny Tags API
  slug: canny-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-tags-api-openapi.yml
- filename: canny-users-api-openapi.yml
  format: yaml
  label: Canny Users API
  slug: canny-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-users-api-openapi.yml
- filename: canny-votes-api-openapi.yml
  format: yaml
  label: Canny Votes API
  slug: canny-votes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-votes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Canny Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canny secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Canny
provider_slug: canny
scheme_count: 2
schemes:
- description: 'Secret API key. Canny documents the key as a body parameter named

    `apiKey`; it is modeled here as an `apiKey` security scheme.'
  in: query
  name: apiKeyBody
  parameter: apiKey
  sources:
  - openapi/canny-openapi.yml
  type: apiKey
- in: header
  name: apiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/canny-openapi.yml
  type: apiKey
slug: canny-authentication
source_filename: canny-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canny-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyBody\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: |-\n    Secret API key. Canny documents the key as a body parameter named\n    `apiKey`; it is modeled here as an `apiKey` security scheme.\n  sources:\n  - openapi/canny-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/canny-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/authentication/canny-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Customer Feedback
- Product Management
- Feature Requests
- Roadmap
- Changelog
- Voice of Customer
- Software-as-a-Service
---
