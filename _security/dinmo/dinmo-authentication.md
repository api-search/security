---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Dinmo Authentication
name_suffix: Authentication
oauth_flows: []
overview: DinMo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DinMo
provider_slug: dinmo
scheme_count: 1
schemes:
- description: 'A DinMo Personalization API key is sent in the HTTP Authorization header as a Bearer token (Authorization: Bearer <API_KEY>). Keys are generated in the DinMo app and scoped to a workspace''s exposed model records. A missing or invalid key returns 401.'
  format: Bearer <API_KEY>
  key_management:
    console_path: Settings > API keys (app.dinmo.io)
    create: Settings > API keys > Add API key
    expiry: not documented
    rotation: DinMo instructs customers to rotate keys regularly and delete keys that are no longer needed; keys can also be reached from the exposure that created the endpoint.
    scope: Read access to the workspace's Personalization API records.
    source: https://docs.dinmo.io/customer-hub/profiles-api/set-up.md
    storage_guidance: Store the key in a server-side secret manager. DinMo explicitly warns against exposing keys in browser or mobile application code and directs calls to a trusted backend or edge function.
  location: header
  name: PersonalizationApiKey
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.dinmo.io/customer-hub/profiles-api/api-reference
  - https://docs.dinmo.io/customer-hub/profiles-api/set-up.md
  - https://docs.dinmo.io/customer-hub/profiles-api.md
  type: http
slug: dinmo-authentication
source_filename: dinmo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.dinmo.io/customer-hub/profiles-api/api-reference\ndocs: https://docs.dinmo.io/customer-hub/profiles-api/api-reference\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  http_schemes:\n  - bearer\nschemes:\n- name: PersonalizationApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    A DinMo Personalization API key is sent in the HTTP Authorization header as a\n    Bearer token (Authorization: Bearer <API_KEY>). Keys are generated in the DinMo\n    app and scoped to a workspace's exposed model records. A missing or invalid key\n    returns 401.\n  location: header\n  parameter: Authorization\n  format: Bearer <API_KEY>\n  key_management:\n    console_path: Settings > API keys (app.dinmo.io)\n    create: Settings > API keys > Add API key\n    scope: Read access to the workspace's Personalization API records.\n    rotation: >-\n      DinMo instructs customers to rotate keys regularly and\
  \ delete keys that are\n      no longer needed; keys can also be reached from the exposure that created\n      the endpoint.\n    storage_guidance: >-\n      Store the key in a server-side secret manager. DinMo explicitly warns against\n      exposing keys in browser or mobile application code and directs calls to a\n      trusted backend or edge function.\n    expiry: not documented\n    source: https://docs.dinmo.io/customer-hub/profiles-api/set-up.md\n  sources:\n  - https://docs.dinmo.io/customer-hub/profiles-api/api-reference\n  - https://docs.dinmo.io/customer-hub/profiles-api/set-up.md\n  - https://docs.dinmo.io/customer-hub/profiles-api.md\nplatform_authentication:\n  surface: DinMo web application (app.dinmo.io)\n  methods:\n  - email/password sign-in\n  - Enterprise SSO (SAML/OIDC) via Google Workspace, Okta, or Microsoft Entra ID\n  rbac: Users, roles and permissions are managed per workspace; audit logs are available.\n  api_relevance: >-\n    SSO governs human access to the\
  \ application, not programmatic API access. There\n    is no OAuth authorization-code flow, no token endpoint, and no scope model for\n    the public API.\n  sources:\n  - https://docs.dinmo.io/workspace-management/enterprise-single-sign-on-sso.md\n  - https://docs.dinmo.io/workspace-management/managing-users-roles-and-permissions.md\nenablement_gate: >-\n  The Personalization API is a native destination that must be enabled for a\n  workspace by DinMo before any key can be used — programmatic access begins with a\n  request to a DinMo representative, not with self-serve key creation.\nnotes: >-\n  Platform access (data sources, destinations, segments) is configured through the\n  DinMo web app; the documented programmatic surface is the Personalization API,\n  which uses Bearer [example key] authentication. No OAuth2 or OpenID Connect flow is\n  documented for the public API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dinmo/refs/heads/main/authentication/dinmo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Customer Data Platform
- CDP
- Reverse ETL
- Data Activation
- Data Warehouse
- Audience Segmentation
- Marketing
- Personalization
- MarTech
---
