---
api_key_in:
- header
api_specs:
- filename: callrail-accounts-api-openapi.yml
  format: yaml
  label: CallRail Accounts API
  slug: callrail-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/openapi/callrail-accounts-api-openapi.yml
- filename: callrail-calls-api-openapi.yml
  format: yaml
  label: CallRail Calls API
  slug: callrail-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/openapi/callrail-calls-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: CallRail runs two distinct authentication models. The v3 REST API uses a user-scoped API key sent in a non-standard Authorization header format. The hosted MCP server uses OAuth 2.0 against CallRail with no API key at all. Neither surface publishes OAuth metadata, an OIDC discovery document, or a scope reference.
kind: authentication
layout: security
method: searched
name: Callrail Authentication
name_suffix: Authentication
oauth_flows:
- unpublished
overview: CallRail secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the unpublished flow(s).
provider_name: CallRail
provider_slug: callrail
scheme_count: 2
schemes:
- applies_to: every v3 REST endpoint
  description: Rails-style token authentication. The value is not a bare token and not `Bearer` — it is the literal string `Token token="..."`, which is the single most common integration mistake against this API.
  format: 'Authorization: Token token="YOUR_API_KEY"'
  in: header
  key_creation: Requires a CallRail account; the key is created in the application before any API call can be made.
  name: TokenAuth
  parameter: Authorization
  revocation: Managed in the CallRail application; not exposed through the API.
  scope_model: 'Keys are scoped to an individual CallRail user and carry exactly that user''s visibility. Responses only include data the user can see in the CallRail interface — calls to accounts or companies the user cannot access are not returned. There are no permission scopes to request, narrow, or grant: a key is as powerful as its user.'
  sources:
  - openapi/callrail-accounts-api-openapi.yml
  - openapi/callrail-calls-api-openapi.yml
  type: apiKey
  warning: 'CallRail''s own warning: "Treat your API key as you would your password... anyone who has your API key can use that key to access or modify any data you have control over."'
- description: The MCP server authenticates the end user with OAuth 2.0 against CallRail — the assistant redirects to CallRail's login page for authorization. No API keys are involved; the session is scoped to the CallRail user account and respects existing account/company permissions.
  detail: mcp/callrail-mcp.yml
  flows: []
  flows_note: Grant type, authorization URL, token URL and scopes are all unpublished. No /.well-known/oauth-authorization-server (RFC 8414) or /.well-known/oauth-protected-resource (RFC 9728) document is reachable, and the MCP endpoint host itself is issued per account, so the flow cannot be discovered programmatically.
  name: MCP OAuth
  sources:
  - https://apidocs.callrail.com/#mcp
  surface: hosted MCP server
  type: oauth2
slug: callrail-authentication
source_filename: callrail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/callrail-accounts-api-openapi.yml, openapi/callrail-calls-api-openapi.yml\ndocs: https://apidocs.callrail.com/#authorization\ndescription: >-\n  CallRail runs two distinct authentication models. The v3 REST API uses a user-scoped API key sent\n  in a non-standard Authorization header format. The hosted MCP server uses OAuth 2.0 against\n  CallRail with no API key at all. Neither surface publishes OAuth metadata, an OIDC discovery\n  document, or a scope reference.\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - unpublished\nschemes:\n  - name: TokenAuth\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Authorization: Token token=\"YOUR_API_KEY\"'\n    description: >-\n      Rails-style token authentication. The value is not a bare token and not `Bearer` — it is the\n      literal string `Token token=\"...\"`, which is the single most common\
  \ integration mistake\n      against this API.\n    applies_to: every v3 REST endpoint\n    sources:\n      - openapi/callrail-accounts-api-openapi.yml\n      - openapi/callrail-calls-api-openapi.yml\n    scope_model: >-\n      Keys are scoped to an individual CallRail user and carry exactly that user's visibility.\n      Responses only include data the user can see in the CallRail interface — calls to accounts or\n      companies the user cannot access are not returned. There are no permission scopes to request,\n      narrow, or grant: a key is as powerful as its user.\n    revocation: Managed in the CallRail application; not exposed through the API.\n    key_creation: >-\n      Requires a CallRail account; the key is created in the application before any API call can be\n      made.\n    warning: >-\n      CallRail's own warning: \"Treat your API key as you would your password... anyone who has your\n      API key can use that key to access or modify any data you have control over.\"\
  \n  - name: MCP OAuth\n    type: oauth2\n    surface: hosted MCP server\n    description: >-\n      The MCP server authenticates the end user with OAuth 2.0 against CallRail — the assistant\n      redirects to CallRail's login page for authorization. No API keys are involved; the session\n      is scoped to the CallRail user account and respects existing account/company permissions.\n    flows: []\n    flows_note: >-\n      Grant type, authorization URL, token URL and scopes are all unpublished. No\n      /.well-known/oauth-authorization-server (RFC 8414) or /.well-known/oauth-protected-resource\n      (RFC 9728) document is reachable, and the MCP endpoint host itself is issued per account, so\n      the flow cannot be discovered programmatically.\n    sources:\n      - https://apidocs.callrail.com/#mcp\n    detail: mcp/callrail-mcp.yml\nrequest_identification:\n  header: Request-From\n  required: false\n  description: >-\n    Not authentication, but CallRail asks third-party platforms\
  \ building integrations to identify\n    themselves with a `Request-From` header carrying their lowercased software name with\n    underscores for spaces (e.g. `Request-From: hanks_hotdogs`). Customers calling the API for\n    their own data do not need it.\n  source: https://apidocs.callrail.com/#identifying-your-integration\nscopes:\n  published: false\n  note: >-\n    No OAuth scopes, permission strings, or scoped-key types are documented for either surface, so\n    no scopes/ artifact is written. Authorization is entirely inherited from the underlying user.\ntransport_security:\n  https_required: true\n  tls: >-\n    api.callrail.com negotiates TLS 1.2 and does not send HSTS; see\n    security/callrail-domain-security.yml.\ngaps:\n  - No scoped or least-privilege API keys — a key inherits its user's full access.\n  - No OAuth for the REST API, so third-party integrations must ask customers to paste a key.\n  - No published OAuth metadata for the MCP server despite it being an OAuth\
  \ surface.\n  - No key rotation, expiry, or last-used visibility documented through the API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callrail/refs/heads/main/authentication/callrail-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Call Tracking
- Conversation Intelligence
- Marketing Attribution
- Lead Tracking
- Telephony
- Analytics
- Form Tracking
---
