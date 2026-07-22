---
api_key_in:
- header
api_specs:
- filename: tesslio-openapi-original.json
  format: json
  label: Tessl API
  slug: tessl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesslio/refs/heads/main/openapi/tesslio-openapi-original.json
auth_types:
- http-bearer
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tesslio Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: tessl.io secures its APIs with http-bearer, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: tessl.io
provider_slug: tesslio
scheme_count: 4
schemes:
- description: API requests to api.tessl.io are authorized with a bearer token in the Authorization header. Interactive users obtain one via `tessl login`; automation uses a workspace API key exported as TESSL_TOKEN.
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/tesslio-openapi-original.json
  type: http
- description: Workspace-scoped API keys created per workspace with a role and optional expiry; used in CI by setting TESSL_TOKEN.
  expiry: optional ISO-8601 expiry date per key
  in: header
  management:
    api: POST /v1/orgs/{orgId}/api-keys, POST /v1/experimental/workspaces/{workspaceId}/api-keys
    create: tessl api-key create
    delete: tessl api-key delete
    list: tessl api-key list
  name: workspaceApiKey
  parameter: Authorization
  roles:
  - member
  - publisher
  - manager
  - owner
  scope: workspace
  token_env: TESSL_TOKEN
  type: apiKey
- authorizationUrl: https://auth.tessl.io/device
  description: '`tessl login` runs an OAuth 2.0 device-authorization flow at auth.tessl.io/device; the user confirms a device code in the browser after signing in with GitHub or Google. Enterprise SSO is available for orgs.'
  flow: deviceCode
  identity_providers:
  - GitHub
  - Google
  name: deviceAuthorization
  type: oauth2
- description: Organization-level Single Sign-On for enterprise accounts.
  docs: https://docs.tessl.io/administrators/sso
  name: sso
  scope: organization
  type: openIdConnect
slug: tesslio-authentication
source_filename: tesslio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tessl.io/introduction-to-tessl/set-up-tessl/installation\ndocs: https://docs.tessl.io/administrators/sso\nnote: >-\n  The published OpenAPI (https://api.tessl.io/openapi.json) does not declare\n  components.securitySchemes; every operation instead accepts an Authorization\n  request-header parameter. The auth model below is captured from the Tessl docs\n  and CLI reference rather than derived from the spec.\nsummary:\n  types:\n  - http-bearer\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - deviceCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    API requests to api.tessl.io are authorized with a bearer token in the\n    Authorization header. Interactive users obtain one via `tessl login`;\n    automation uses a workspace API key exported as TESSL_TOKEN.\n  sources:\n  - openapi/tesslio-openapi-original.json\n\
  - name: workspaceApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  token_env: TESSL_TOKEN\n  scope: workspace\n  roles:\n  - member\n  - publisher\n  - manager\n  - owner\n  management:\n    create: tessl api-key create\n    list: tessl api-key list\n    delete: tessl api-key delete\n    api: POST /v1/orgs/{orgId}/api-keys, POST /v1/experimental/workspaces/{workspaceId}/api-keys\n  expiry: optional ISO-8601 expiry date per key\n  description: >-\n    Workspace-scoped API keys created per workspace with a role and optional\n    expiry; used in CI by setting TESSL_TOKEN.\n- name: deviceAuthorization\n  type: oauth2\n  flow: deviceCode\n  authorizationUrl: https://auth.tessl.io/device\n  identity_providers:\n  - GitHub\n  - Google\n  description: >-\n    `tessl login` runs an OAuth 2.0 device-authorization flow at\n    auth.tessl.io/device; the user confirms a device code in the browser after\n    signing in with GitHub or Google. Enterprise SSO is available for orgs.\n\
  - name: sso\n  type: openIdConnect\n  scope: organization\n  docs: https://docs.tessl.io/administrators/sso\n  description: Organization-level Single Sign-On for enterprise accounts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesslio/refs/heads/main/authentication/tesslio-authentication.yml
summary_line: http-bearer/apiKey/oauth2 · 4 schemes
tags:
- Company
- Ai Ml
- Agent Enablement
- Agentic Development
- Developer Tools
- Skills Registry
- Model Context Protocol
- Spec-Driven Development
- Code Review
- CLI
---
