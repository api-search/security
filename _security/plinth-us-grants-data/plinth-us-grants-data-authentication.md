---
api_key_in:
- header
api_specs:
- filename: plinth-us-grants-data-analyze-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Analyze API
  slug: plinth-us-grants-data-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-analyze-api-openapi.yml
- filename: plinth-us-grants-data-grants-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Grants API
  slug: plinth-us-grants-data-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-grants-api-openapi.yml
- filename: plinth-us-grants-data-organizations-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Organizations API
  slug: plinth-us-grants-data-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-organizations-api-openapi.yml
- filename: plinth-us-grants-data-resolve-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data Resolve API
  slug: plinth-us-grants-data-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-resolve-api-openapi.yml
- filename: plinth-us-grants-data-sql-api-openapi.yml
  format: yaml
  label: Plinth US Grants Data SQL API
  slug: plinth-us-grants-data-sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/openapi/plinth-us-grants-data-sql-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Plinth Us Grants Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plinth US Grants Data secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Plinth US Grants Data
provider_slug: plinth-us-grants-data
scheme_count: 2
schemes:
- alternative_evidence: '"Send your key in an X-API-Key header (or as a Authorization: Bearer token — both work)" (/developers#auth). NOTE: only X-API-Key is declared in the OpenAPI — the Bearer form is documented but not in the contract, so a generated client will only know the header form.'
  alternative_form: Bearer <key>
  alternative_parameter: Authorization
  applied: global
  applied_evidence: 'Root-level `security: [{ApiKeyAuth: []}]` in the OpenAPI, with a per-operation override on searchOrganizations.'
  env_var: PLINTH_API_KEY
  env_var_source: /.well-known/api-onboarding (authentication.methods[0].env)
  handling_guidance: '"Keys are secrets — keep them server-side, never in browser JavaScript, a mobile binary or a committed file." (/developers#auth)'
  in: header
  issuance:
    cost: free tier requires no card
    keys_per_account: 1
    mechanism: console-only
    note: '"The REST key is minted by a signed-in human at /account (one key per account, rotatable, shown once). There is no programmatic issue endpoint." — /.well-known/api-onboarding.'
    one_time_display: true
    programmatic: false
    sign_in: Google sign-in or an email link
    url: https://data.useplinth.com/account
  name: ApiKeyAuth
  parameter: X-API-Key
  rotation:
    note: '"Rotating retires the previous key immediately." No overlap window — plan for a hard cutover.'
    semantics: immediate-revoke
    supported: true
    url: https://data.useplinth.com/account
  sources:
  - https://data.useplinth.com/developers#auth
  - openapi/plinth-us-grants-data-openapi.json
  surface: REST (https://data.useplinth.com/api)
  token_prefix: plinth_sk_
  token_prefix_source: /developers#auth ("it starts plinth_sk_") and /.well-known/api-onboarding (authentication.methods[0].tokenPrefix).
  ttl: none
  type: apiKey
- authorization_endpoint: https://data.useplinth.com/oauth/authorize
  bearer_methods:
  - header
  challenge_observed:
    checked: '2026-08-14'
    header: 'www-authenticate: Bearer error="invalid_token", error_description="No authorization provided", resource_metadata="https://data.useplinth.com/.well-known/oauth-protected-resource"'
    status: 401
    url: https://data.useplinth.com/api/connector/mcp
  declared_in_openapi: false
  declared_in_openapi_note: The REST OpenAPI does not model this scheme — correctly, since it protects a different surface. It is discoverable only from the RFC 8414 metadata document.
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://data.useplinth.com
  metadata: well-known/plinth-us-grants-data-oauth-authorization-server.json
  name: ConnectorOAuth
  pkce: S256
  profile: OAuth 2.1 (authorization_code + PKCE S256), public client
  protected_resource_metadata: well-known/plinth-us-grants-data-oauth-protected-resource.json
  registration_endpoint: https://data.useplinth.com/oauth/register
  revocation: Remove the connector in the assistant, or revoke from https://data.useplinth.com/account.
  scopes:
  - plinth:read
  see: scopes/plinth-us-grants-data-scopes.yml
  sources:
  - https://data.useplinth.com/connect
  - https://data.useplinth.com/.well-known/oauth-authorization-server
  surface: MCP (https://data.useplinth.com/api/connector/mcp)
  token_endpoint: https://data.useplinth.com/oauth/token
  token_endpoint_auth_methods:
  - none
  token_ttl: short-lived; refresh_token grant supported
  type: oauth2
slug: plinth-us-grants-data-authentication
source_filename: plinth-us-grants-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://data.useplinth.com/developers#auth\ncorroboration:\n  - openapi/plinth-us-grants-data-openapi.json          # components.securitySchemes.ApiKeyAuth\n  - https://data.useplinth.com/.well-known/api-onboarding\n  - https://data.useplinth.com/.well-known/oauth-authorization-server\nderived_baseline: derive-authentication.py (2026-08-14) — upgraded to `searched` with the docs and onboarding descriptor.\nchecked: '2026-08-14'\n\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  note: >-\n    TWO independent auth systems on one host, and they do not overlap. The REST API takes a static\n    API key in a header. The MCP connector takes OAuth 2.1 with PKCE and dynamic client\n    registration. A REST key will not authenticate the connector and an OAuth token is not\n    documented for REST. One operation — GET /api/search — is deliberately unauthenticated.\n\nschemes:\n  - name: ApiKeyAuth\n    surface: REST (https://data.useplinth.com/api)\n\
  \    type: apiKey\n    in: header\n    parameter: X-API-Key\n    alternative_parameter: Authorization\n    alternative_form: 'Bearer <key>'\n    alternative_evidence: >-\n      \"Send your key in an X-API-Key header (or as a Authorization: Bearer token — both work)\"\n      (/developers#auth). NOTE: only X-API-Key is declared in the OpenAPI — the Bearer form is\n      documented but not in the contract, so a generated client will only know the header form.\n    token_prefix: plinth_sk_\n    token_prefix_source: >-\n      /developers#auth (\"it starts plinth_sk_\") and /.well-known/api-onboarding\n      (authentication.methods[0].tokenPrefix).\n    env_var: PLINTH_API_KEY\n    env_var_source: /.well-known/api-onboarding (authentication.methods[0].env)\n    applied: global\n    applied_evidence: 'Root-level `security: [{ApiKeyAuth: []}]` in the OpenAPI, with a per-operation override on searchOrganizations.'\n    issuance:\n      mechanism: console-only\n      url: https://data.useplinth.com/account\n\
  \      programmatic: false\n      cost: free tier requires no card\n      sign_in: Google sign-in or an email link\n      one_time_display: true\n      keys_per_account: 1\n      note: >-\n        \"The REST key is minted by a signed-in human at /account (one key per account, rotatable,\n        shown once). There is no programmatic issue endpoint.\" — /.well-known/api-onboarding.\n    rotation:\n      supported: true\n      url: https://data.useplinth.com/account\n      semantics: immediate-revoke\n      note: '\"Rotating retires the previous key immediately.\" No overlap window — plan for a hard cutover.'\n    ttl: none\n    handling_guidance: >-\n      \"Keys are secrets — keep them server-side, never in browser JavaScript, a mobile binary or a\n      committed file.\" (/developers#auth)\n    sources:\n      - https://data.useplinth.com/developers#auth\n      - openapi/plinth-us-grants-data-openapi.json\n\n  - name: ConnectorOAuth\n    surface: MCP (https://data.useplinth.com/api/connector/mcp)\n\
  \    type: oauth2\n    profile: OAuth 2.1 (authorization_code + PKCE S256), public client\n    declared_in_openapi: false\n    declared_in_openapi_note: >-\n      The REST OpenAPI does not model this scheme — correctly, since it protects a different\n      surface. It is discoverable only from the RFC 8414 metadata document.\n    metadata: well-known/plinth-us-grants-data-oauth-authorization-server.json\n    protected_resource_metadata: well-known/plinth-us-grants-data-oauth-protected-resource.json\n    issuer: https://data.useplinth.com\n    authorization_endpoint: https://data.useplinth.com/oauth/authorize\n    token_endpoint: https://data.useplinth.com/oauth/token\n    registration_endpoint: https://data.useplinth.com/oauth/register\n    dynamic_client_registration: true\n    grant_types: [authorization_code, refresh_token]\n    pkce: S256\n    token_endpoint_auth_methods: [none]\n    bearer_methods: [header]\n    scopes: [plinth:read]\n    see: scopes/plinth-us-grants-data-scopes.yml\n\
  \    token_ttl: short-lived; refresh_token grant supported\n    revocation: 'Remove the connector in the assistant, or revoke from https://data.useplinth.com/account.'\n    challenge_observed:\n      url: https://data.useplinth.com/api/connector/mcp\n      status: 401\n      header: >-\n        www-authenticate: Bearer error=\"invalid_token\", error_description=\"No authorization\n        provided\", resource_metadata=\"https://data.useplinth.com/.well-known/oauth-protected-resource\"\n      checked: '2026-08-14'\n    sources:\n      - https://data.useplinth.com/connect\n      - https://data.useplinth.com/.well-known/oauth-authorization-server\n\nanonymous_surface:\n  operation: searchOrganizations\n  path: GET /api/search\n  security: []\n  metered: false\n  evidence: >-\n    Per-operation `security: []` in the OpenAPI overrides the global requirement, and the spec says\n    so in prose: \"**No API key required and not metered.**\" Verified live 2026-08-14: GET\n    /api/search?q=barancik\
  \ returned 200 with a result body and no auth header sent.\n  significance: >-\n    Rare and agent-friendly. Entity resolution — the step that must precede every other call when\n    you have a name rather than an EIN — is free, unkeyed and unmetered. An agent can resolve\n    \"Barancik Foundation\" to EIN 363442474 and a canonical URL before it needs any credential at\n    all. Plinth's own onboarding descriptor calls this \"the intended first call.\"\n\nagent_readiness_notes:\n  can_an_agent_self_provision: false\n  blocker: >-\n    A human must sign in at /account to mint the REST key, and must hold the For consultants plan\n    before the MCP consent step can succeed. The provider documents both as gaps in its own\n    onboarding descriptor rather than leaving an agent to discover them at a 401.\n  strongest_signal: >-\n    The credential requirements are published as MACHINE-READABLE data, not prose: token prefix,\n    env var name, rotation semantics, one-time display, plan gates\
  \ and the registration mechanisms\n    all live in /.well-known/api-onboarding. Very few providers in the catalog publish this.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plinth-us-grants-data/refs/heads/main/authentication/plinth-us-grants-data-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Philanthropy
- Grants
- Nonprofits
- Foundations
- IRS 990
- Open Data
- Government Spending
- Research
- Agents
- REST
- JSON
- MCP
- SQL
---
