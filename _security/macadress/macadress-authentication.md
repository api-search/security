---
api_key_in:
- header
- query
- body
api_specs:
- filename: macadress-openapi.yaml
  format: yaml
  label: macadress.com API
  slug: macadresscom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/openapi/macadress-openapi.yaml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Macadress Authentication
name_suffix: Authentication
oauth_flows: []
overview: 'MAC Address Lookup: Find Vendor, OUI & Device Type secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.'
provider_name: 'MAC Address Lookup: Find Vendor, OUI & Device Type'
provider_slug: macadress
scheme_count: 3
schemes:
- applies_to: all operations
  format: 'Authorization: Bearer mk_...'
  header: Authorization
  in: header
  name: apiKeyHeader
  preferred: true
  scheme: bearer
  sources:
  - openapi/macadress-openapi.yaml
  - https://macadress.com/docs
  type: http
- applies_to: all operations
  caution: 'A key in the query string is written into proxy logs, server access logs, browser history and Referer headers. Documented as a convenience, not the recommended transport.

    '
  format: ?api_key=mk_...
  in: query
  name: apiKeyQuery
  parameter: api_key
  preferred: false
  sources:
  - openapi/macadress-openapi.yaml
  - https://macadress.com/docs
  type: apiKey
- applies_to:
  - lookupMACBatch
  declared_in_openapi: true
  format: an "api_key" field alongside "macs" in the JSON body
  in: body
  name: apiKeyBody
  note: 'Documented as a third transport and present as a request-body property, but not modelled as a securityScheme (OpenAPI cannot express a body-borne credential as one). A strict spec-driven client will not know it exists.

    '
  openapi_location: paths./v1/mac/batch.post.requestBody.content.application/json.schema.properties.api_key
  parameter: api_key
  sources:
  - https://macadress.com/docs
  type: apiKey
slug: macadress-authentication
source_filename: macadress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://macadress.com/docs\ndocs:\n- https://macadress.com/docs\n- https://macadress.com/mcp\nderived_from:\n- openapi/macadress-openapi.yaml\nsummary:\n  model: static API key\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  - body\n  key_prefix: mk_\n  oauth: false\n  oidc: false\n  mtls: false\n  signup: https://macadress.com/signup\n  provisioning: >\n    Instant and self-serve. A free key is created the moment an account is created, with no\n    approval step, and is visible any time on the account page. Only the browser lookup tool\n    on macadress.com is usable without a key; the REST API and the MCP server both require one.\nschemes:\n- name: apiKeyHeader\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer mk_...'\n  applies_to: all operations\n  preferred: true\n  sources:\n  - openapi/macadress-openapi.yaml\n  - https://macadress.com/docs\n\
  - name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  format: '?api_key=mk_...'\n  applies_to: all operations\n  preferred: false\n  caution: >\n    A key in the query string is written into proxy logs, server access logs, browser\n    history and Referer headers. Documented as a convenience, not the recommended transport.\n  sources:\n  - openapi/macadress-openapi.yaml\n  - https://macadress.com/docs\n- name: apiKeyBody\n  type: apiKey\n  in: body\n  parameter: api_key\n  applies_to: [lookupMACBatch]\n  format: 'an \"api_key\" field alongside \"macs\" in the JSON body'\n  declared_in_openapi: true\n  openapi_location: paths./v1/mac/batch.post.requestBody.content.application/json.schema.properties.api_key\n  note: >\n    Documented as a third transport and present as a request-body property, but not modelled\n    as a securityScheme (OpenAPI cannot express a body-borne credential as one). A strict\n    spec-driven client will not know it exists.\n  sources:\n  - https://macadress.com/docs\n\
  anonymous_operations:\n- operationId: healthz\n  path: /v1/healthz\n  openapi_declaration: 'security: []'\n  note: Liveness only. Not counted against any quota.\nunauthenticated_behaviour:\n  status: 401\n  body: '{\"error\": \"missing API key: pass it as \\\"api_key\\\" (query param or POST body) or an Authorization: Bearer header\"}'\n  www_authenticate_header: false\n  observed_live: '2026-08-28'\n  note: >\n    The 401 body names all three accepted transports, which is unusually helpful. No\n    WWW-Authenticate challenge is emitted, so a client cannot negotiate the scheme from the\n    response alone.\nmcp_authentication:\n  endpoint: https://mcp.macadress.com/mcp\n  scheme: http bearer, same mk_ key as REST\n  oauth: false\n  probed: '2026-08-28 POST tools/list -> 401 \"no bearer token\"'\n  provider_rationale: >\n    Stated on https://macadress.com/mcp: MCP's authorization spec is optional for HTTP\n    transports, and the provider chose a spec-legal bearer token over standing up\
  \ a full\n    OAuth 2.1 authorization server with PKCE and dynamic client registration. Consequence\n    for agents: no one-click \"connect your account\" flow, and no\n    /.well-known/oauth-protected-resource to discover.\nkey_management:\n  rotation_policy: not published\n  scopes: none\n  multiple_keys: not published\n  revocation: not published\n  gap: >\n    No published guidance on rotating, revoking or issuing multiple keys, and no scope or\n    permission model — one key carries the account's full read surface and its whole\n    billing quota. For an agent deployment that is the practical blast radius: a leaked key\n    cannot be narrowed, only replaced.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/authentication/macadress-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Networking
- Network Access Control
- Security
- SecOps
- IoT
- Device Fleet Management
- MDM
- Reference Data
- IEEE OUI Lookup
- Developer Tools
- MCP
- agent-native
---
