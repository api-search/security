---
api_key_in:
- header
api_specs:
- filename: fullcontact-address-api-openapi.yml
  format: yaml
  label: FullContact Address API
  slug: fullcontact-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-address-api-openapi.yml
- filename: fullcontact-audience-api-openapi.yml
  format: yaml
  label: FullContact Audience API
  slug: fullcontact-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-audience-api-openapi.yml
- filename: fullcontact-enrich-api-openapi.yml
  format: yaml
  label: FullContact Enrich API
  slug: fullcontact-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-enrich-api-openapi.yml
- filename: fullcontact-identity-api-openapi.yml
  format: yaml
  label: FullContact Identity API
  slug: fullcontact-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-identity-api-openapi.yml
- filename: fullcontact-permission-api-openapi.yml
  format: yaml
  label: FullContact Permission API
  slug: fullcontact-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-permission-api-openapi.yml
- filename: fullcontact-tags-api-openapi.yml
  format: yaml
  label: FullContact Tags API
  slug: fullcontact-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-tags-api-openapi.yml
auth_types:
- http
description: 'One credential covers everything FullContact exposes: the V3 REST API and the hosted MCP server both authenticate with the same API key, sent as an HTTP Bearer token. There is no OAuth, no OIDC, no separate MCP credential, and no scope surface — entitlements are attached to the key by FullContact''s account team rather than requested by the client.'
kind: authentication
layout: security
method: searched
name: Fullcontact Authentication
name_suffix: Authentication
oauth_flows: []
overview: FullContact secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FullContact
provider_slug: fullcontact
scheme_count: 1
schemes:
- description: FullContact API key passed as a Bearer token in the Authorization header.
  format: Bearer <your-fullcontact-api-key>
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fullcontact-openapi.yml
  - https://docs.fullcontact.com/docs/authentication
  type: http
slug: fullcontact-authentication
source_filename: fullcontact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/fullcontact-openapi.yml\ndocs: https://docs.fullcontact.com/docs/generate-an-api-key\ndescription: >-\n  One credential covers everything FullContact exposes: the V3 REST API and the\n  hosted MCP server both authenticate with the same API key, sent as an HTTP\n  Bearer token. There is no OAuth, no OIDC, no separate MCP credential, and no\n  scope surface — entitlements are attached to the key by FullContact's account\n  team rather than requested by the client.\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: FullContact API key passed as a Bearer token in the Authorization header.\n  header: Authorization\n  format: 'Bearer <your-fullcontact-api-key>'\n  sources:\n  - openapi/fullcontact-openapi.yml\n  - https://docs.fullcontact.com/docs/authentication\n\nkey_management:\n  provisioning: https://docs.fullcontact.com/docs/generate-an-api-key\n\
  \  console: https://platform.fullcontact.com\n  key_types:\n    - {type: production, note: required for production traffic}\n    - {type: sandbox, note: '\"accepted for evaluation only\"'}\n  entitlements: >-\n    Products are entitled per key by FullContact, not requested per call. A key\n    must have person.enrich enabled to use the MCP server; a key without it\n    receives 403 forbidden and the fix is to contact the FullContact account\n    team.\n  rotation: >-\n    Generate a new key in the developer dashboard, update every client, then\n    revoke the old key. FullContact holds no server-side cache of the key, so\n    the next request uses the new value immediately.\n  multi_client: >-\n    A single key can be used across multiple clients simultaneously; all calls\n    count against the same rate limit and quota.\n\nmcp:\n  endpoint: https://api.fullcontact.com/v3/mcp\n  scheme: same Bearer API key\n  oauth: false\n  docs: https://docs.fullcontact.com/docs/authentication\n  note:\
  \ >-\n    \"There is no separate MCP credential, no OAuth flow, and no need to\n    provision new accounts.\"\n\nfailure_modes:\n  - {status: 401, code: unauthorized, cause: Missing or malformed Authorization header, surface: mcp}\n  - {status: 403, code: forbidden, cause: Key lacks the person.enrich entitlement, surface: mcp}\n  - {status: 403, cause: 'API key invalid, missing, or over quota / rate-limit', surface: rest}\n\nnot_published:\n  - OAuth 2.0 or OpenID Connect flows\n  - scopes / permission strings (see conformance — no OAuthScopes artifact is emitted)\n  - mTLS\n  - key prefixes that distinguish sandbox from production\n  - '/.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource (both 404)'\n\nx-evidence:\n  - fetched: '2026-08-14'\n    url: https://docs.fullcontact.com/docs/authentication.md\n    http_status: 200\n  - fetched: '2026-08-14'\n    url: https://api.fullcontact.com/.well-known/oauth-authorization-server\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/authentication/fullcontact-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity Resolution
- Customer Data
- Data Enrichment
- Person API
- Company API
- Privacy-Safe Identity
- Customer Recognition
---
