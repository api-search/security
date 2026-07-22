---
api_key_in:
- header
api_specs:
- filename: tl-dv-openapi.yml
  format: yaml
  label: tl;dv API
  slug: tldv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tl Dv Authentication
name_suffix: Authentication
oauth_flows: []
overview: tl;dv secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: tl;dv
provider_slug: tl-dv
scheme_count: 1
schemes:
- description: 'All requests authenticate with an API key sent on the x-api-key header. Keys are issued per user from tl;dv account settings and can be scoped to user, team, or organization context.

    '
  in: header
  key_management_url: https://tldv.io/app/settings/personal-settings/api-keys
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/tl-dv-openapi.yml
  type: apiKey
slug: tl-dv-authentication
source_filename: tl-dv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://doc.tldv.io\ndocs: https://doc.tldv.io\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_names: [x-api-key]\n  oauth2_flows: []\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: >\n      All requests authenticate with an API key sent on the x-api-key header.\n      Keys are issued per user from tl;dv account settings and can be scoped to\n      user, team, or organization context.\n    key_management_url: https://tldv.io/app/settings/personal-settings/api-keys\n    sources: [openapi/tl-dv-openapi.yml]\nnotes: >\n  tl;dv uses a single API-key model (no OAuth2/OIDC scope surface), so a scopes/\n  artifact is intentionally omitted. Health check (GET /v1alpha1/health) is the\n  only unauthenticated operation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/authentication/tl-dv-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI
- Meetings
- Transcription
- Notetaking
- Conversation Intelligence
- Productivity
- Video
- Webhooks
- API
---
