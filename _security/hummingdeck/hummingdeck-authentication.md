---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hummingdeck-companies-api-openapi.yml
  format: yaml
  label: HummingDeck Companies API
  slug: hummingdeck-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-companies-api-openapi.yml
- filename: hummingdeck-contacts-api-openapi.yml
  format: yaml
  label: HummingDeck Contacts API
  slug: hummingdeck-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-contacts-api-openapi.yml
- filename: hummingdeck-decisions-api-openapi.yml
  format: yaml
  label: HummingDeck Decisions API
  slug: hummingdeck-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-decisions-api-openapi.yml
- filename: hummingdeck-decks-api-openapi.yml
  format: yaml
  label: HummingDeck Decks API
  slug: hummingdeck-decks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-decks-api-openapi.yml
- filename: hummingdeck-emails-api-openapi.yml
  format: yaml
  label: HummingDeck Emails API
  slug: hummingdeck-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-emails-api-openapi.yml
- filename: hummingdeck-hooks-api-openapi.yml
  format: yaml
  label: HummingDeck Hooks API
  slug: hummingdeck-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-hooks-api-openapi.yml
- filename: hummingdeck-me-api-openapi.yml
  format: yaml
  label: HummingDeck Me API
  slug: hummingdeck-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-me-api-openapi.yml
- filename: hummingdeck-room-labels-api-openapi.yml
  format: yaml
  label: HummingDeck Room Labels API
  slug: hummingdeck-room-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-room-labels-api-openapi.yml
- filename: hummingdeck-room-views-api-openapi.yml
  format: yaml
  label: HummingDeck Room Views API
  slug: hummingdeck-room-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-room-views-api-openapi.yml
- filename: hummingdeck-rooms-api-openapi.yml
  format: yaml
  label: HummingDeck Rooms API
  slug: hummingdeck-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-rooms-api-openapi.yml
- filename: hummingdeck-shares-api-openapi.yml
  format: yaml
  label: HummingDeck Shares API
  slug: hummingdeck-shares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-shares-api-openapi.yml
- filename: hummingdeck-views-api-openapi.yml
  format: yaml
  label: HummingDeck Views API
  slug: hummingdeck-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hummingdeck/openapi/hummingdeck-views-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Hummingdeck Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: HummingDeck secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: HummingDeck
provider_slug: hummingdeck
scheme_count: 2
schemes:
- bearerFormat: hd_api_...
  description: Named workspace API key issued by a workspace owner or admin. Prefixed hd_api_, shown once at creation, valid for one year, independently scoped and revoked, and bound permanently to its workspace. Each *:write scope includes the matching *:read capability. Not accepted on webhook subscription endpoints.
  name: apiToken
  scheme: bearer
  sources:
  - openapi/hummingdeck-openapi.json
  type: http
- description: Issued by the Zapier integration's OAuth flow. Access tokens last 30 days; refresh tokens last 90 days. The only credential accepted on webhook subscription endpoints.
  flows:
  - authorizationUrl: https://app.hummingdeck.com/api/zapier/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://app.hummingdeck.com/api/zapier/token
  name: oauth2
  sources:
  - openapi/hummingdeck-openapi.json
  type: oauth2
slug: hummingdeck-authentication
source_filename: hummingdeck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: derived\nsource: openapi/hummingdeck-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  bearerFormat: hd_api_...\n  description: Named workspace API key issued by a workspace owner or admin. Prefixed hd_api_,\n    shown once at creation, valid for one year, independently scoped and revoked, and bound\n    permanently to its workspace. Each *:write scope includes the matching *:read capability.\n    Not accepted on webhook subscription endpoints.\n  sources:\n  - openapi/hummingdeck-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hummingdeck.com/api/zapier/authorize\n    tokenUrl: https://app.hummingdeck.com/api/zapier/token\n    scopes: 0\n  description: Issued by the Zapier integration's OAuth flow. Access tokens last 30 days; refresh\n    tokens last 90 days. The only\
  \ credential accepted on webhook subscription endpoints.\n  sources:\n  - openapi/hummingdeck-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hummingdeck/authentication/hummingdeck-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Document Sharing
- Engagement Analytics
- Digital Sales Rooms
- Data Rooms
- Client Portals
- Integrations
- Secure Sharing
---
