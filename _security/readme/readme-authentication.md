---
api_key_in: []
api_specs:
- filename: readme-personalized-docs-webhook-asyncapi.yml
  format: yaml
  label: ReadMe Personalized Docs Webhook
  slug: personalized-docs-webhook
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/asyncapi/readme-personalized-docs-webhook-asyncapi.yml
- filename: readme-analytics-api-openapi.yml
  format: yaml
  label: ReadMe Analytics API
  slug: readme-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-analytics-api-openapi.yml
- filename: readme-api-keys-api-openapi.yml
  format: yaml
  label: ReadMe API Keys API
  slug: readme-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-api-keys-api-openapi.yml
- filename: readme-apis-api-openapi.yml
  format: yaml
  label: ReadMe APIs API
  slug: readme-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-apis-api-openapi.yml
- filename: readme-branches-api-openapi.yml
  format: yaml
  label: ReadMe Branches API
  slug: readme-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-branches-api-openapi.yml
- filename: readme-categories-api-openapi.yml
  format: yaml
  label: ReadMe Categories API
  slug: readme-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-categories-api-openapi.yml
- filename: readme-changelog-api-openapi.yml
  format: yaml
  label: ReadMe Changelog API
  slug: readme-changelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-changelog-api-openapi.yml
- filename: readme-custom-pages-api-openapi.yml
  format: yaml
  label: ReadMe Custom Pages API
  slug: readme-custom-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-custom-pages-api-openapi.yml
- filename: readme-guides-api-openapi.yml
  format: yaml
  label: ReadMe Guides API
  slug: readme-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-guides-api-openapi.yml
- filename: readme-images-api-openapi.yml
  format: yaml
  label: ReadMe Images API
  slug: readme-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-images-api-openapi.yml
- filename: readme-metrics-api-openapi.yml
  format: yaml
  label: ReadMe Metrics API
  slug: readme-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-metrics-api-openapi.yml
- filename: readme-recipes-api-openapi.yml
  format: yaml
  label: ReadMe Recipes API
  slug: readme-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-recipes-api-openapi.yml
- filename: readme-search-api-openapi.yml
  format: yaml
  label: ReadMe Search API
  slug: readme-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Readme Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReadMe secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ReadMe
provider_slug: readme
scheme_count: 2
schemes:
- description: HTTP Basic auth using your ReadMe API key as the username (password blank).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/readme-developer-metrics-openapi.yml
  type: http
- description: Use your ReadMe API key as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/readme-openapi.yml
  type: http
slug: readme-authentication
source_filename: readme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/readme-developer-metrics-openapi.yml, openapi/readme-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using your ReadMe API key as the username (password blank).\n  sources:\n  - openapi/readme-developer-metrics-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Use your ReadMe API key as a Bearer token in the Authorization header.\n  sources:\n  - openapi/readme-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/authentication/readme-authentication.yml
summary_line: http · 2 schemes
tags:
- Documentation
- Developer Hub
- API Reference
- Portals
- Analytics
- AI
- MCP
- Bi-Directional Sync
---
