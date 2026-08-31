---
api_key_in: []
api_specs:
- filename: flora-fauna-actions-api-openapi.yml
  format: yaml
  label: FLORA Actions API
  slug: flora-fauna-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-actions-api-openapi.yml
- filename: flora-fauna-assets-api-openapi.yml
  format: yaml
  label: FLORA Assets API
  slug: flora-fauna-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-assets-api-openapi.yml
- filename: flora-fauna-canvas-api-openapi.yml
  format: yaml
  label: FLORA Canvas API
  slug: flora-fauna-canvas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-canvas-api-openapi.yml
- filename: flora-fauna-feedback-api-openapi.yml
  format: yaml
  label: FLORA Feedback API
  slug: flora-fauna-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-feedback-api-openapi.yml
- filename: flora-fauna-generations-api-openapi.yml
  format: yaml
  label: FLORA Generations API
  slug: flora-fauna-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-generations-api-openapi.yml
- filename: flora-fauna-models-api-openapi.yml
  format: yaml
  label: FLORA Models API
  slug: flora-fauna-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-models-api-openapi.yml
- filename: flora-fauna-projects-api-openapi.yml
  format: yaml
  label: FLORA Projects API
  slug: flora-fauna-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-projects-api-openapi.yml
- filename: flora-fauna-runs-api-openapi.yml
  format: yaml
  label: FLORA Runs API
  slug: flora-fauna-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-runs-api-openapi.yml
- filename: flora-fauna-technique-runs-api-openapi.yml
  format: yaml
  label: FLORA Technique Runs API
  slug: flora-fauna-technique-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-technique-runs-api-openapi.yml
- filename: flora-fauna-techniques-api-openapi.yml
  format: yaml
  label: FLORA Techniques API
  slug: flora-fauna-techniques-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-techniques-api-openapi.yml
- filename: flora-fauna-workspaces-api-openapi.yml
  format: yaml
  label: FLORA Workspaces API
  slug: flora-fauna-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/openapi/flora-fauna-workspaces-api-openapi.yml
auth_types:
- http
- oauth2
description: FLORA runs two independent authentication paths against the same workspace and the same billing. The REST API takes a bearer API key; the MCP server takes OAuth 2.1 with PKCE and will NOT accept the API key. The docs state plainly that they can be used in parallel, and that the audit trail differs — an API key attributes an action to a service account, OAuth attributes it to a named human in a named client.
kind: authentication
layout: security
method: searched
name: Flora Fauna Authentication
name_suffix: Authentication
oauth_flows: []
overview: FLORA secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FLORA
provider_slug: flora-fauna
scheme_count: 3
schemes:
- creation: FLORA app > Settings > API Keys (https://app.flora.ai/projects?openSettings=true&initialTab=apiKeys)
  header: 'Authorization: Bearer sk_live_XXXX'
  key_prefixes:
    production: sk_live_
    sandbox: sk_test_
  keys_per_workspace: 1
  name: bearerAuth
  permissions_model: Inherits the permissions of the workspace the key was created in. Read everything, create runs (billed), upload assets, create/modify projects if the workspace allows. Never billing or member management.
  revocation: immediate; subsequent requests return 401 invalid_api_key
  rotation:
    note: 'A hard operational constraint worth flagging: exactly one active key per workspace with NO overlap window means every production rotation is a cutover, not a drain. The docs offer to enable a hot-swap window per workspace on request to support.'
    overlap_window: false
    procedure: create the new key, cut applications over, then revoke the old one
  sandbox_caveat: The docs qualify sk_test_ as "sandbox, when available" — no separate sandbox base URL or test-mode environment is published, so treat test keys as not generally available.
  scheme: bearer
  scopes: null
  scopes_note: The REST API publishes no scope vocabulary; a key is workspace-wide.
  secret_visibility: shown once at creation
  sources:
  - openapi/flora-fauna-flora-api-openapi.yml
  - https://developer.flora.ai/platform/authentication
  surface: REST API (https://app.flora.ai/api/v1)
  type: http
- authorization_endpoint: https://agents.flora.ai/authorize
  authorization_server: https://agents.flora.ai
  discovery:
    rfc8414: well-known/flora-fauna-agents-oauth-authorization-server.json
    rfc9728: well-known/flora-fauna-agents-oauth-protected-resource-mcp.json
  dynamic_client_registration: true
  error_on_expiry: 401 invalid_token
  grant_types:
  - authorization_code
  - refresh_token
  name: mcp-oauth
  pkce:
  - S256
  - plain
  registration_endpoint: https://agents.flora.ai/register
  revocation: FLORA app > Settings > Connected apps, per client
  revocation_endpoint: https://agents.flora.ai/token
  scopes: null
  scopes_note: 'scopes_supported is absent from the authorization-server metadata. Access is described in role terms instead: the connection gets exactly what the signed-in FLORA user has in the connected workspace, and never billing or member management.'
  sources:
  - https://developer.flora.ai/mcp/authentication
  - well-known/flora-fauna-well-known.yml
  surface: MCP server (https://agents.flora.ai/mcp)
  token_endpoint: https://agents.flora.ai/token
  token_storage: in the MCP client; FLORA does not hold client tokens
  type: oauth2
  version: OAuth 2.1
- discovery: well-known/flora-fauna-app-openid-configuration.json
  id_token_signing_alg: RS256
  issuer: https://clerk.flora.ai
  name: clerk-application-oidc
  note: Clerk-hosted end-user identity for the product itself. Recorded because it is genuinely served from a FLORA host and enumerates scopes, but it is NOT the API's authentication and an integrator should not build against it.
  pkce:
  - S256
  scopes:
  - openid
  - profile
  - email
  - public_metadata
  - private_metadata
  - offline_access
  sources:
  - well-known/flora-fauna-app-openid-configuration.json
  surface: FLORA application sign-in (https://app.florafauna.ai)
  type: openIdConnect
slug: flora-fauna-authentication
source_filename: flora-fauna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  Baseline derived from openapi/flora-fauna-flora-api-openapi.yml\n  (components.securitySchemes), then upgraded from FLORA's own documentation:\n  https://developer.flora.ai/platform/authentication and\n  https://developer.flora.ai/mcp/authentication, plus live probes of the OAuth\n  discovery documents in well-known/.\ndocs:\n  - https://developer.flora.ai/platform/authentication\n  - https://developer.flora.ai/mcp/authentication\ndescription: >-\n  FLORA runs two independent authentication paths against the same workspace and\n  the same billing. The REST API takes a bearer API key; the MCP server takes\n  OAuth 2.1 with PKCE and will NOT accept the API key. The docs state plainly\n  that they can be used in parallel, and that the audit trail differs — an API key\n  attributes an action to a service account, OAuth attributes it to a named human\n  in a named client.\nsummary:\n  types: [http, oauth2]\n  primary: http-bearer\n\
  \  mfa_or_delegated: oauth2 (MCP only)\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    surface: REST API (https://app.flora.ai/api/v1)\n    header: 'Authorization: Bearer sk_live_XXXX'\n    key_prefixes:\n      production: sk_live_\n      sandbox: sk_test_\n    sandbox_caveat: >-\n      The docs qualify sk_test_ as \"sandbox, when available\" — no separate sandbox\n      base URL or test-mode environment is published, so treat test keys as not\n      generally available.\n    creation: FLORA app > Settings > API Keys (https://app.flora.ai/projects?openSettings=true&initialTab=apiKeys)\n    secret_visibility: shown once at creation\n    keys_per_workspace: 1\n    rotation:\n      overlap_window: false\n      procedure: create the new key, cut applications over, then revoke the old one\n      note: >-\n        A hard operational constraint worth flagging: exactly one active key per\n        workspace with NO overlap window means every production rotation is a\n \
  \       cutover, not a drain. The docs offer to enable a hot-swap window per\n        workspace on request to support.\n    revocation: immediate; subsequent requests return 401 invalid_api_key\n    permissions_model: >-\n      Inherits the permissions of the workspace the key was created in. Read\n      everything, create runs (billed), upload assets, create/modify projects if\n      the workspace allows. Never billing or member management.\n    scopes: null\n    scopes_note: The REST API publishes no scope vocabulary; a key is workspace-wide.\n    sources:\n      - openapi/flora-fauna-flora-api-openapi.yml\n      - https://developer.flora.ai/platform/authentication\n  - name: mcp-oauth\n    type: oauth2\n    surface: MCP server (https://agents.flora.ai/mcp)\n    version: OAuth 2.1\n    grant_types: [authorization_code, refresh_token]\n    pkce: [S256, plain]\n    dynamic_client_registration: true\n    authorization_server: https://agents.flora.ai\n    authorization_endpoint: https://agents.flora.ai/authorize\n\
  \    token_endpoint: https://agents.flora.ai/token\n    registration_endpoint: https://agents.flora.ai/register\n    revocation_endpoint: https://agents.flora.ai/token\n    discovery:\n      rfc8414: well-known/flora-fauna-agents-oauth-authorization-server.json\n      rfc9728: well-known/flora-fauna-agents-oauth-protected-resource-mcp.json\n    scopes: null\n    scopes_note: >-\n      scopes_supported is absent from the authorization-server metadata. Access is\n      described in role terms instead: the connection gets exactly what the\n      signed-in FLORA user has in the connected workspace, and never billing or\n      member management.\n    token_storage: in the MCP client; FLORA does not hold client tokens\n    revocation: FLORA app > Settings > Connected apps, per client\n    error_on_expiry: 401 invalid_token\n    sources:\n      - https://developer.flora.ai/mcp/authentication\n      - well-known/flora-fauna-well-known.yml\n  - name: clerk-application-oidc\n    type: openIdConnect\n\
  \    surface: FLORA application sign-in (https://app.florafauna.ai)\n    issuer: https://clerk.flora.ai\n    discovery: well-known/flora-fauna-app-openid-configuration.json\n    scopes: [openid, profile, email, public_metadata, private_metadata, offline_access]\n    id_token_signing_alg: RS256\n    pkce: [S256]\n    note: >-\n      Clerk-hosted end-user identity for the product itself. Recorded because it is\n      genuinely served from a FLORA host and enumerates scopes, but it is NOT the\n      API's authentication and an integrator should not build against it.\n    sources:\n      - well-known/flora-fauna-app-openid-configuration.json\ntransport_security:\n  https_required: true\n  webhook_callback_https_required: true\n  note: >-\n    Webhook callback_url values must be HTTPS and are rejected if they resolve to\n    localhost, *.local/*.internal, cloud-metadata hostnames, or private/loopback/\n    link-local IPs; FLORA does not follow 3xx on delivery.\nsecret_handling_guidance:\n \
  \ server_side_only: true\n  env_var: FLORA_API_KEY\n  webhook_secret_env: FLORA_WEBHOOK_SECRET\n  rotation_cadence_recommended: 90 days\n  published_at: https://developer.flora.ai/platform/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flora-fauna/refs/heads/main/authentication/flora-fauna-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Creative AI
- Generative AI
- Infinite Canvas
- Node-Based Workflows
- Creative Workspace
- Image-Generation
- Video Generation
- Text-to-Image
- Text-to-Video
- AI Agents
- Multimodal AI
- Design Tools
- Creative Professionals
- Advertising
- Film
- Fashion
- Branding
- VFX
- Photography
- Architecture
- Motion Design
- FAUNA
- MCP
- Agent Tools
- Workflow-Automation
---
