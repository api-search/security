---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Autoura Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Autoura secures its APIs with apiKey, http, oauth2, and openIdConnect across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Autoura
provider_slug: autoura
scheme_count: 6
schemes:
- applies_to: the REST API (https://api.autoura.com/api)
  audience: brands, designers, suppliers, affiliates
  description: 'A static API key sent as "Authorization: Bearer <API_KEY>". Keys are issued in the Autoura Dashboard, on the first page after sign-in under "Your account". Autoura states that not all keys are equal -- "Brands are the most powerful (for retail), designers for example can''t access preferences & personalisation tools" -- so the key itself carries the authorisation tier.'
  key_posture:
    client_side_use: permitted
    provider_statement: '"The API key is expected to be used within mobile apps and other client side code (e.g. JavaScript). There is no method to access customer details or other GDPR related information with these API keys."'
    sharing: Each service must use its own key; Autoura asks that keys are not committed to public repositories or shared between organisations.
  name: bearerApiKey
  probe:
    checked: '2026-09-13'
    unauthenticated_body: '{"success":false, "error_title": "Missing authorization header", "error_message": "Please configure an authorization header with your API key"}'
    unauthenticated_status: 401
    url: https://api.autoura.com/api/whoami
  scheme: bearer
  source: https://www.autoura.com/docs/api/authentication
  type: http
  verification_endpoint: https://api.autoura.com/api/whoami
  verification_note: Autoura publishes WhoAmI specifically as the auth test because it is the one endpoint not served from the Fastly cache -- a cached endpoint can appear to work when the credential is wrong.
- applies_to: the MCP endpoint (https://api.autoura.com/api/mcp)
  audience: AI agents
  description: OAuth 2.1-shaped authorization-code flow with PKCE and dynamic client registration, advertised through a conformant RFC 9728 protected-resource document and an RFC 8414 authorization-server document.
  discovery:
  - well-known/autoura-oauth-protected-resource.json
  - well-known/autoura-oauth-authorization-server.json
  - well-known/autoura-openid-configuration.json
  flows:
  - authorizationUrl: https://api.autoura.com/api/auth/oauth2/authorize
    flow: authorizationCode
    jwksUri: https://api.autoura.com/api/auth/oauth2/jwks
    pkce: S256
    registrationUrl: https://api.autoura.com/api/auth/oauth2/register
    scopes:
      files:read: read scope advertised for the MCP resource
      files:write: write scope advertised for the MCP resource
      offline_access: refresh-token scope (OIDC document only)
    tokenUrl: https://api.autoura.com/api/auth/oauth2/token
  issuer: https://api.autoura.com/api/auth
  name: mcpOAuth2
  probe:
    checked: '2026-09-13'
    method: POST
    unauthenticated_status: 401
    url: https://api.autoura.com/api/mcp
    www_authenticate: Bearer resource_metadata="https://api.autoura.com/api/.well-known/oauth-protected-resource", scope="files:read"
  protected_resource: https://api.autoura.com/api/mcp
  source: https://api.autoura.com/api/.well-known/oauth-protected-resource
  type: oauth2
- applies_to: the same authorization server as mcpOAuth2
  description: 'An OIDC discovery document is served alongside the OAuth one. It is the richer of the two: it adds refresh_token to grant_types_supported, offline_access to scopes_supported, subject_types_supported [public] and id_token_signing_alg_values_supported [RS256].'
  name: openIdConnect
  openIdConnectUrl: https://api.autoura.com/api/auth/.well-known/openid-configuration
  source: well-known/autoura-openid-configuration.json
  type: openIdConnect
- applies_to: the MCP endpoint, for agents onboarding a human account
  audience: consumer AI agents acting for a named human
  code_lifetime: 60 minutes
  concurrency: Issuing a new token does not invalidate previous ones; multiple unexpired tokens can coexist.
  description: A second, non-OAuth route to an MCP bearer token, documented for agents. Three open POST endpoints -- /api/identity/open/register, /api/identity/open/signin_code_send and /api/identity/open/verify -- exchange a six-digit email code for an access_token. The token always represents the HUMAN account owner and carries a DID for that human, even when the agent authenticated with its own pai_email.
  identity_model:
    human_email: required -- the account owner
    note: In Autoura B2B the PAI is its own user, "separate from the human user ... not attached to the human as a profile field or sub-identity".
    pai_email: optional -- the Personal AI's own authentication email
  name: emailCodeBearer
  scheme: bearer
  source: https://www.planmyvisit.to/docs/ai/authentication.md
  token_lifetime: 48 hours
  type: http
- applies_to: PlanMyVisit WebMCP pages
  description: Browser-session authentication for WebMCP. The website session resolves the trusted profile; a browser-supplied profile ID is never trusted. The server mints a short-lived internal MCP credential with a five-minute lifetime to call the same tools, which limits replay without shortening the human's website session. Agent self-registration is not available here.
  name: webMcpSession
  source: https://www.planmyvisit.to/docs/ai/authentication.md
  type: session
- applies_to: the consumer preference and location services
  description: Autoura publishes DID Documents for consumer profiles and, since 22 October 2024, an AI agent definition inside them. A DIDCommMessaging service (version 2) in a counterparty DID Document lets an external agent exchange DIDComm messages; Autoura resolves through the DIF Universal Resolver only.
  name: didcomm
  source: https://www.autoura.com/docs/api/profiles/didcomm
  type: decentralized-identity
slug: autoura-authentication
source_filename: autoura-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://www.autoura.com/docs/api/authentication\ndocs:\n  - https://www.autoura.com/docs/api/authentication\n  - https://www.autoura.com/core/pai/docs/authentication.md\n  - https://www.planmyvisit.to/docs/ai/authentication.md\nnote: >-\n  Autoura publishes no OpenAPI, so nothing here is derived from securitySchemes.\n  Every scheme below was read from the provider's own authentication pages and,\n  where possible, confirmed against a live probe. Autoura runs THREE distinct\n  authentication models on one API host, for three distinct audiences, and the\n  docs say so explicitly (\"Authentication is handled differently for the MCP\n  endpoint\").\nsummary:\n  types: [apiKey, http, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  distinct_models: 3\nschemes:\n  - name: bearerApiKey\n    type: http\n    scheme: bearer\n    applies_to: the REST API (https://api.autoura.com/api)\n    audience:\
  \ brands, designers, suppliers, affiliates\n    description: >-\n      A static API key sent as \"Authorization: Bearer <API_KEY>\". Keys are issued in\n      the Autoura Dashboard, on the first page after sign-in under \"Your account\".\n      Autoura states that not all keys are equal -- \"Brands are the most powerful\n      (for retail), designers for example can't access preferences & personalisation\n      tools\" -- so the key itself carries the authorisation tier.\n    key_posture:\n      client_side_use: permitted\n      provider_statement: >-\n        \"The API key is expected to be used within mobile apps and other client side\n        code (e.g. JavaScript). There is no method to access customer details or\n        other GDPR related information with these API keys.\"\n      sharing: >-\n        Each service must use its own key; Autoura asks that keys are not committed\n        to public repositories or shared between organisations.\n    verification_endpoint: https://api.autoura.com/api/whoami\n\
  \    verification_note: >-\n      Autoura publishes WhoAmI specifically as the auth test because it is the one\n      endpoint not served from the Fastly cache -- a cached endpoint can appear to\n      work when the credential is wrong.\n    probe:\n      url: https://api.autoura.com/api/whoami\n      unauthenticated_status: 401\n      unauthenticated_body: '{\"success\":false, \"error_title\": \"Missing authorization header\", \"error_message\": \"Please configure an authorization header with your API key\"}'\n      checked: '2026-09-13'\n    source: https://www.autoura.com/docs/api/authentication\n  - name: mcpOAuth2\n    type: oauth2\n    applies_to: the MCP endpoint (https://api.autoura.com/api/mcp)\n    audience: AI agents\n    description: >-\n      OAuth 2.1-shaped authorization-code flow with PKCE and dynamic client\n      registration, advertised through a conformant RFC 9728 protected-resource\n      document and an RFC 8414 authorization-server document.\n    flows:\n      -\
  \ flow: authorizationCode\n        authorizationUrl: https://api.autoura.com/api/auth/oauth2/authorize\n        tokenUrl: https://api.autoura.com/api/auth/oauth2/token\n        registrationUrl: https://api.autoura.com/api/auth/oauth2/register\n        jwksUri: https://api.autoura.com/api/auth/oauth2/jwks\n        pkce: S256\n        scopes:\n          files:read: read scope advertised for the MCP resource\n          files:write: write scope advertised for the MCP resource\n          offline_access: refresh-token scope (OIDC document only)\n    issuer: https://api.autoura.com/api/auth\n    protected_resource: https://api.autoura.com/api/mcp\n    discovery:\n      - well-known/autoura-oauth-protected-resource.json\n      - well-known/autoura-oauth-authorization-server.json\n      - well-known/autoura-openid-configuration.json\n    probe:\n      url: https://api.autoura.com/api/mcp\n      method: POST\n      unauthenticated_status: 401\n      www_authenticate: 'Bearer resource_metadata=\"\
  https://api.autoura.com/api/.well-known/oauth-protected-resource\", scope=\"files:read\"'\n      checked: '2026-09-13'\n    source: https://api.autoura.com/api/.well-known/oauth-protected-resource\n  - name: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://api.autoura.com/api/auth/.well-known/openid-configuration\n    applies_to: the same authorization server as mcpOAuth2\n    description: >-\n      An OIDC discovery document is served alongside the OAuth one. It is the richer\n      of the two: it adds refresh_token to grant_types_supported, offline_access to\n      scopes_supported, subject_types_supported [public] and\n      id_token_signing_alg_values_supported [RS256].\n    source: well-known/autoura-openid-configuration.json\n  - name: emailCodeBearer\n    type: http\n    scheme: bearer\n    applies_to: the MCP endpoint, for agents onboarding a human account\n    audience: consumer AI agents acting for a named human\n    description: >-\n      A second, non-OAuth\
  \ route to an MCP bearer token, documented for agents.\n      Three open POST endpoints -- /api/identity/open/register,\n      /api/identity/open/signin_code_send and /api/identity/open/verify -- exchange a\n      six-digit email code for an access_token. The token always represents the\n      HUMAN account owner and carries a DID for that human, even when the agent\n      authenticated with its own pai_email.\n    token_lifetime: 48 hours\n    code_lifetime: 60 minutes\n    concurrency: >-\n      Issuing a new token does not invalidate previous ones; multiple unexpired\n      tokens can coexist.\n    identity_model:\n      human_email: required -- the account owner\n      pai_email: optional -- the Personal AI's own authentication email\n      note: >-\n        In Autoura B2B the PAI is its own user, \"separate from the human user ...\n        not attached to the human as a profile field or sub-identity\".\n    source: https://www.planmyvisit.to/docs/ai/authentication.md\n  - name: webMcpSession\n\
  \    type: session\n    applies_to: PlanMyVisit WebMCP pages\n    description: >-\n      Browser-session authentication for WebMCP. The website session resolves the\n      trusted profile; a browser-supplied profile ID is never trusted. The server\n      mints a short-lived internal MCP credential with a five-minute lifetime to\n      call the same tools, which limits replay without shortening the human's\n      website session. Agent self-registration is not available here.\n    source: https://www.planmyvisit.to/docs/ai/authentication.md\n  - name: didcomm\n    type: decentralized-identity\n    applies_to: the consumer preference and location services\n    description: >-\n      Autoura publishes DID Documents for consumer profiles and, since 22 October\n      2024, an AI agent definition inside them. A DIDCommMessaging service (version 2)\n      in a counterparty DID Document lets an external agent exchange DIDComm messages;\n      Autoura resolves through the DIF Universal Resolver\
  \ only.\n    source: https://www.autoura.com/docs/api/profiles/didcomm\nconsent_model:\n  note: >-\n    Consumer preference data is not reachable with an API key alone. Autoura brokers\n    it: POST /api/identity/share/invite returns an identity_invite_key rendered as a\n    QR code, the consumer scans it in the Autoura Connect app, and only after state\n    becomes share_permission_given does the polling endpoint return preferences.\n    Scope is negotiated per invite (scope, scope_location of no/approximate/accurate,\n    scope_companions of no/match/discovery_aggregate). A profile_jwt grants\n    subsequent access for 7 days and excludes companion data.\n  docs: https://www.autoura.com/docs/api/integrations/signin\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoura/refs/heads/main/authentication/autoura-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 6 schemes
tags:
- Tourism
- Tours
- Travel
- Destination
- Experience
- Digital Tourism
---
