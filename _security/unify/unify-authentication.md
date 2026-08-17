---
api_key_in:
- header
api_specs:
- filename: unify-events-api-openapi.yml
  format: yaml
  label: Unify Analytics Events API
  slug: unify-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-events-api-openapi.yml
- filename: unify-event-query-jobs-api-openapi.yml
  format: yaml
  label: Unify Event Query Jobs API
  slug: unify-event-query-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-event-query-jobs-api-openapi.yml
- filename: unify-objects-api-openapi.yml
  format: yaml
  label: Unify Objects API
  slug: unify-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-objects-api-openapi.yml
- filename: unify-object-attributes-api-openapi.yml
  format: yaml
  label: Unify Object Attributes API
  slug: unify-object-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-attributes-api-openapi.yml
- filename: unify-object-attribute-options-api-openapi.yml
  format: yaml
  label: Unify Object Attribute Options API
  slug: unify-object-attribute-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-attribute-options-api-openapi.yml
- filename: unify-object-records-api-openapi.yml
  format: yaml
  label: Unify Object Records API
  slug: unify-object-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-records-api-openapi.yml
- filename: unify-object-record-query-jobs-api-openapi.yml
  format: yaml
  label: Unify Object Record Query Jobs API
  slug: unify-object-record-query-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-record-query-jobs-api-openapi.yml
- filename: unify-sequences-api-openapi.yml
  format: yaml
  label: Unify Sequences API
  slug: unify-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequences-api-openapi.yml
- filename: unify-sequence-enrollments-api-openapi.yml
  format: yaml
  label: Unify Sequence Enrollments API
  slug: unify-sequence-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequence-enrollments-api-openapi.yml
- filename: unify-sequence-enrollment-steps-api-openapi.yml
  format: yaml
  label: Unify Sequence Enrollment Steps API
  slug: unify-sequence-enrollment-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequence-enrollment-steps-api-openapi.yml
- filename: unify-tasks-api-openapi.yml
  format: yaml
  label: Unify Tasks API
  slug: unify-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-tasks-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Unify Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- clientCredentials
- refreshToken
- tokenExchange
overview: Unify secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, clientCredentials, refreshToken, and tokenExchange flow(s).
provider_name: Unify
provider_slug: unify
scheme_count: 3
schemes:
- applies_to:
  - Data API
  - Sequences API
  - Tasks API
  in: header
  name: ApiKeyAuth
  operations: 65
  parameter: x-api-key
  provisioning: Generated in the Unify app under Settings -> Developers (app.unifygtm.com/dashboard/settings/integrations/api-keys).
  scope_note: A key carries the full authority of the Unify user it belongs to. No read-only key, no per-resource key, no expiry policy is published. The Bulk API specifically requires a user-backed API key.
  scoped: false
  sources:
  - openapi/_original/unify-data-openapi.json
  - openapi/_original/unify-sequences-openapi.json
  - openapi/_original/unify-tasks-openapi.json
  type: apiKey
- applies_to:
  - Analytics API
  detail: HTTP Basic with a public write key, intended for client-side collection from a browser or product. Write-only ingest, which is why a publishable credential is acceptable here.
  name: BasicAuth
  operations: 3
  scheme: Basic
  sources:
  - openapi/_original/unify-analytics-openapi.json
  type: http
- alternative: An x-api-key header may be sent to the MCP endpoint instead of an OAuth bearer token, for clients that cannot run the browser login.
  bearer_methods:
  - header
  cross_link: scopes/unify-scopes.yml
  declared_in_openapi: false
  discovery:
    authorization_server: https://auth.unifygtm.com/
    protected_resource: https://mcp.unifygtm.com/.well-known/oauth-protected-resource/mcp
    spec:
    - RFC 9728
    - RFC 8414
    - OpenID Connect Discovery 1.0
  dynamic_client_registration: true
  evidence:
    checked: '2026-08-13'
    http_status: 401
    probe: POST tools/list to https://mcp.unifygtm.com/mcp
    www_authenticate: Bearer resource_metadata="https://mcp.unifygtm.com/.well-known/oauth-protected-resource/mcp", error="invalid_request", error_description="No authentication token provided."
  issuer: https://auth.unifygtm.com/
  name: MCP OAuth
  pkce:
  - S256
  - plain
  platform: Auth0 on a Unify custom domain
  scopes: identity only (openid, profile, email, offline_access, ...) - no product scopes
  surface: https://mcp.unifygtm.com/mcp
  type: oauth2
slug: unify-authentication
source_filename: unify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  openapi/_original/unify-analytics-openapi.json,\n  openapi/_original/unify-data-openapi.json,\n  openapi/_original/unify-sequences-openapi.json,\n  openapi/_original/unify-tasks-openapi.json\n  (harvested live 2026-08-13),\n  https://mcp.unifygtm.com/.well-known/oauth-protected-resource/mcp,\n  https://auth.unifygtm.com/.well-known/oauth-authorization-server\ndocs: https://docs.unifygtm.com/developers/introduction\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\n    - deviceCode\n    - clientCredentials\n    - refreshToken\n    - tokenExchange\n  oauth2_surface: MCP only (not declared in any OpenAPI)\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    applies_to: [Data API, Sequences API, Tasks API]\n    operations: 65\n    sources:\n      - openapi/_original/unify-data-openapi.json\n      -\
  \ openapi/_original/unify-sequences-openapi.json\n      - openapi/_original/unify-tasks-openapi.json\n    provisioning: >-\n      Generated in the Unify app under Settings -> Developers\n      (app.unifygtm.com/dashboard/settings/integrations/api-keys).\n    scoped: false\n    scope_note: >-\n      A key carries the full authority of the Unify user it belongs to. No\n      read-only key, no per-resource key, no expiry policy is published. The Bulk\n      API specifically requires a user-backed API key.\n  - name: BasicAuth\n    type: http\n    scheme: Basic\n    applies_to: [Analytics API]\n    operations: 3\n    sources:\n      - openapi/_original/unify-analytics-openapi.json\n    detail: >-\n      HTTP Basic with a public write key, intended for client-side collection from\n      a browser or product. Write-only ingest, which is why a publishable\n      credential is acceptable here.\n  - name: MCP OAuth\n    type: oauth2\n    declared_in_openapi: false\n    surface: https://mcp.unifygtm.com/mcp\n\
  \    discovery:\n      protected_resource: https://mcp.unifygtm.com/.well-known/oauth-protected-resource/mcp\n      authorization_server: https://auth.unifygtm.com/\n      spec: [RFC 9728, RFC 8414, OpenID Connect Discovery 1.0]\n    issuer: https://auth.unifygtm.com/\n    platform: Auth0 on a Unify custom domain\n    bearer_methods: [header]\n    pkce: [S256, plain]\n    dynamic_client_registration: true\n    scopes: identity only (openid, profile, email, offline_access, ...) - no product scopes\n    alternative: >-\n      An x-api-key header may be sent to the MCP endpoint instead of an OAuth\n      bearer token, for clients that cannot run the browser login.\n    cross_link: scopes/unify-scopes.yml\n    evidence:\n      probe: POST tools/list to https://mcp.unifygtm.com/mcp\n      http_status: 401\n      www_authenticate: >-\n        Bearer resource_metadata=\"https://mcp.unifygtm.com/.well-known/oauth-protected-resource/mcp\",\n        error=\"invalid_request\", error_description=\"\
  No authentication token provided.\"\n      checked: '2026-08-13'\nposture:\n  transport: HTTPS only across all hosts (see security/unify-domain-security.yml).\n  mtls: false\n  signed_requests: false\n  key_rotation_policy_published: false\n  sso: >-\n    SSO is offered for the Unify application as a Business-plan add-on; it governs\n    app login, not API authentication.\ngaps:\n  - id: no-least-privilege\n    detail: >-\n      Neither authentication path can express less than full user authority. There\n      are no API-key scopes and no product OAuth scopes, so delegating a\n      narrow capability to an agent is not possible - a key or token that can read\n      a record can also delete a sequence.\n  - id: no-key-lifecycle\n    detail: >-\n      No documented key expiry, rotation guidance, or last-used visibility.\nnotes: >-\n  Three of the four APIs authenticate with a single x-api-key header; the fourth\n  (Analytics) uses HTTP Basic with a publishable write key because it is a\n\
  \  browser-side ingest path. OAuth exists only on the MCP surface, where the\n  authorization server is a full Auth0 tenant on Unify's own domain with RFC 9728\n  protected-resource discovery - a notably more modern posture than the REST APIs\n  it fronts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/authentication/unify-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Sales
- Marketing
- Go-To-Market
- Outbound
- Intent Data
- AI Agents
- B2B
- Data Enrichment
- Sequences
- Analytics
- Tasks
- Bulk API
- MCP
- Agent Skills
- Webhooks
---
