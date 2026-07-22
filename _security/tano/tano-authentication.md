---
api_key_in: []
api_specs:
- filename: tano-openapi-original.json
  format: json
  label: Tano Public API
  slug: tano-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tano/refs/heads/main/openapi/tano-openapi-original.json
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Tano Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tano secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tano
provider_slug: tano
scheme_count: 0
schemes: []
slug: tano-authentication
source_filename: tano-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tano.ai/agents.md\ndocs: https://tano.ai/agents.md\nsummary:\n  types: [none]\n  model: public-unauthenticated\n  note: >-\n    Tano's public HTTP API (contact, signups, webinar registration) requires no API key\n    and no OAuth flow - all documented endpoints are open, CORS-enabled JSON endpoints.\n    The OpenAPI declares no securitySchemes. Programmatic management of live creator\n    campaigns is not exposed as a public API; it is delivered as a managed service via a\n    dedicated account manager. Scoped keys for managed-service integrations are issued\n    out of band on request (team@tano.ai).\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tano/refs/heads/main/authentication/tano-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Influencer Marketing
- Creator Economy
- Marketing
- Advertising
- Artificial Intelligence
- Social Media
- TikTok
- Instagram
- Agent Native
---
