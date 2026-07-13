---
api_key_in: []
api_specs:
- filename: miro-openapi.json
  format: json
  label: Miro Boards API
  slug: miro-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Board Items API
  slug: miro-board-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Connectors API
  slug: miro-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Tags API
  slug: miro-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Mind Map API
  slug: miro-mind-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Board Members API
  slug: miro-board-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Webhooks API
  slug: miro-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Organization API
  slug: miro-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Teams API
  slug: miro-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Audit Logs API
  slug: miro-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro SCIM API
  slug: miro-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Web SDK
  slug: miro-web-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Miro Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Miro secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Miro
provider_slug: miro
scheme_count: 1
schemes:
- description: For more information, see https://developers.miro.com/reference/authorization-flow-for-expiring-tokens
  flows:
  - authorizationUrl: https://miro.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://api.miro.com/v1/oauth/token
  name: oAuth2AuthCode
  sources:
  - openapi/miro-openapi.json
  type: oauth2
slug: miro-authentication
source_filename: miro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/miro-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oAuth2AuthCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://miro.com/oauth/authorize\n    tokenUrl: https://api.miro.com/v1/oauth/token\n    scopes: 8\n  description: For more information, see https://developers.miro.com/reference/authorization-flow-for-expiring-tokens\n  sources:\n  - openapi/miro-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/authentication/miro-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Productivity
- Whiteboard
- Visual Collaboration
- Diagramming
- SaaS
---
