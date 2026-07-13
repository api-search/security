---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Fireflies GraphQL API
  slug: fireflies-graphql-api
  spec_type: OpenAPI
  url: https://docs.fireflies.ai/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fireflies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fireflies.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fireflies.ai
provider_slug: fireflies
scheme_count: 1
schemes:
- description: Obtain an API key from the Fireflies dashboard under Settings > Integrations > API. Pass the key as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fireflies-graphql-api-openapi.yml
  type: http
slug: fireflies-authentication
source_filename: fireflies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fireflies-graphql-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Obtain an API key from the Fireflies dashboard under Settings > Integrations\n    > API. Pass the key as a Bearer token in the Authorization header.\n  sources:\n  - openapi/fireflies-graphql-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireflies/refs/heads/main/authentication/fireflies-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Meeting Assistant
- Transcription
- Summaries
- Action Items
- GraphQL
- Meetings
- Productivity
- Collaboration
- Conversation Intelligence
---
