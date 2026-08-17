---
api_key_in: []
api_specs:
- filename: paragraph-analytics-api-openapi.yml
  format: yaml
  label: Paragraph analytics API
  slug: paragraph-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-analytics-api-openapi.yml
- filename: paragraph-auth-api-openapi.yml
  format: yaml
  label: Paragraph auth API
  slug: paragraph-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-auth-api-openapi.yml
- filename: paragraph-coins-api-openapi.yml
  format: yaml
  label: Paragraph coins API
  slug: paragraph-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-coins-api-openapi.yml
- filename: paragraph-discover-api-openapi.yml
  format: yaml
  label: Paragraph discover API
  slug: paragraph-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-discover-api-openapi.yml
- filename: paragraph-emails-api-openapi.yml
  format: yaml
  label: Paragraph emails API
  slug: paragraph-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-emails-api-openapi.yml
- filename: paragraph-me-api-openapi.yml
  format: yaml
  label: Paragraph me API
  slug: paragraph-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-me-api-openapi.yml
- filename: paragraph-posts-api-openapi.yml
  format: yaml
  label: Paragraph posts API
  slug: paragraph-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-posts-api-openapi.yml
- filename: paragraph-publications-api-openapi.yml
  format: yaml
  label: Paragraph publications API
  slug: paragraph-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-publications-api-openapi.yml
- filename: paragraph-subscribers-api-openapi.yml
  format: yaml
  label: Paragraph subscribers API
  slug: paragraph-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-subscribers-api-openapi.yml
- filename: paragraph-users-api-openapi.yml
  format: yaml
  label: Paragraph users API
  slug: paragraph-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/openapi/paragraph-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Paragraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paragraph secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paragraph
provider_slug: paragraph
scheme_count: 1
schemes:
- description: API key for authenticating protected endpoints. Pass as Bearer token in the Authorization header. Applied to the write and account-scoped operations; public reads (search, feed, public publication/post fetch) need no credential.
  key_source: app.paragraph.com → Settings → API keys
  name: apiKey
  scheme: bearer
  sources:
  - openapi/_original/paragraph-openapi-original.json
  - openapi/paragraph-analytics-api-openapi.yml
  - openapi/paragraph-auth-api-openapi.yml
  - openapi/paragraph-coins-api-openapi.yml
  - openapi/paragraph-discover-api-openapi.yml
  - openapi/paragraph-emails-api-openapi.yml
  - openapi/paragraph-me-api-openapi.yml
  - openapi/paragraph-posts-api-openapi.yml
  - openapi/paragraph-publications-api-openapi.yml
  - openapi/paragraph-subscribers-api-openapi.yml
  - openapi/paragraph-users-api-openapi.yml
  transport: 'Authorization: Bearer <api-key>'
  type: http
slug: paragraph-authentication
source_filename: paragraph-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://paragraph.com/auth.md\ndocs: https://docs.paragraph.com/developers\nalso_derived_from:\n  - openapi/_original/paragraph-openapi-original.json\n  - https://paragraph.com/.well-known/oauth-authorization-server\n  - https://paragraph.com/.well-known/oauth-protected-resource\n  - https://mcp.paragraph.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n    - http\n  primary: HTTP Bearer API key\n  fine_grained: false\n  provider_statement: >-\n    \"Paragraph API keys grant read and write access to the publication the user selects during\n    approval. The keys are not currently fine-grained.\" — https://paragraph.com/auth.md\nschemes:\n  - name: apiKey\n    type: http\n    scheme: bearer\n    description: >-\n      API key for authenticating protected endpoints. Pass as Bearer token in the Authorization\n      header. Applied to the write and account-scoped operations; public reads (search, feed,\n      public\
  \ publication/post fetch) need no credential.\n    key_source: app.paragraph.com → Settings → API keys\n    transport: 'Authorization: Bearer <api-key>'\n    sources:\n      - openapi/_original/paragraph-openapi-original.json\n      - openapi/paragraph-analytics-api-openapi.yml\n      - openapi/paragraph-auth-api-openapi.yml\n      - openapi/paragraph-coins-api-openapi.yml\n      - openapi/paragraph-discover-api-openapi.yml\n      - openapi/paragraph-emails-api-openapi.yml\n      - openapi/paragraph-me-api-openapi.yml\n      - openapi/paragraph-posts-api-openapi.yml\n      - openapi/paragraph-publications-api-openapi.yml\n      - openapi/paragraph-subscribers-api-openapi.yml\n      - openapi/paragraph-users-api-openapi.yml\ndiscovery:\n  protected_resource_metadata:\n    url: https://paragraph.com/.well-known/oauth-protected-resource\n    status: 200\n    file: well-known/paragraph-oauth-protected-resource.json\n    spec: RFC 9728\n  authorization_server_metadata:\n    url: https://paragraph.com/.well-known/oauth-authorization-server\n\
  \    status: 200\n    file: well-known/paragraph-oauth-authorization-server.json\n    spec: RFC 8414\n  scopes_supported: [api.read, api.write]\n  note: >-\n    New since the 2026-07-20 round. Paragraph now advertises its API resource through standard\n    OAuth discovery documents even though the credential it ultimately issues is an API key\n    rather than an OAuth access token.\nagent_registration:\n  published_skill: https://paragraph.com/auth.md\n  saved_as: skills/paragraph-auth-SKILL.md\n  model: anonymous registration followed by a human claim\n  steps:\n    - step: discover\n      detail: Read the RFC 9728 / RFC 8414 documents at paragraph.com.\n    - step: register\n      detail: >-\n        POST https://public.api.paragraph.com/api/v1/api/auth/sessions with an optional deviceName\n        (and optional callbackUrl); receives sessionId, verificationUrl and expiresAt.\n      operationId: createAuthSession\n    - step: claim\n      detail: >-\n        Present verificationUrl (https://paragraph.com/api/auth?session=<session-id>)\
  \ to the user,\n        who signs in, selects a publication, and approves access. The agent must not attempt to\n        approve on the user's behalf.\n      operationId: getAuthSession\n    - step: use\n      detail: Send the issued API key as an Authorization Bearer header on subsequent calls.\n  identity_types_supported: [anonymous]\n  credential_types_supported: [api_key]\n  agent_guardrails:\n    - Do not try to approve the request for the user.\n    - Do not expose the returned credential in logs, messages, or source code.\n  assessment: >-\n    A genuinely agent-native auth design: a machine-readable discovery document points at a\n    markdown instruction file written for an agent, and the registration/claim handshake is\n    modelled as three real REST operations with a human approval step in the middle.\nmcp_authorization:\n  issuer: https://mcp.paragraph.com\n  model: OAuth 2.1 authorization code + PKCE, with RFC 7591 dynamic client registration\n  scopes_supported: []\n  browser_flow:\
  \ true\n  local_alternative: PARAGRAPH_API_KEY environment variable for the stdio server\n  note: >-\n    A separate authorization server from the REST resource, advertising no scopes — an MCP grant\n    is coarser than the api.read/api.write split offered on the REST side.\nnot_supported:\n  oauth2_in_spec: >-\n    The OpenAPI declares no oauth2 securityScheme, so no scopes can be derived from the contract\n    itself; they exist only in the discovery documents. See scopes/paragraph-scopes.yml.\n  openid_connect: /.well-known/openid-configuration returns 404 on every host.\n  mtls: not offered\n  http_message_signatures: not offered\ncross_ref:\n  - scopes/paragraph-scopes.yml\n  - well-known/paragraph-well-known.yml\n  - conventions/paragraph-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragraph/refs/heads/main/authentication/paragraph-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Publishing
- Newsletters
- Web3
- Content
- Blogging
- Creator Economy
- API
---
