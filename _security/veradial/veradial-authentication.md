---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: veradial-openapi-generated.yml
  format: yaml
  label: VeraDial Zapier Integration API
  slug: zapier-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veradial/refs/heads/main/openapi/_ae-authored/veradial-openapi-generated.yml
auth_types:
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Veradial Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: VeraDial secures its APIs with http-bearer and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: VeraDial
provider_slug: veradial
scheme_count: 4
schemes:
- applies_to: VeraDial Zapier Integration API (hooks, lines, samples, me)
  description: 'Zapier-facing requests authenticate with Authorization: Bearer vdk_... using an API key generated from the VeraDial Integrations dashboard. The key is a narrow credential: it works only with the hooks, lines, samples, and me endpoints, and its full value is shown once. VeraDial Plus is required to create a key.'
  key_prefix: vdk_
  management: https://app.veradial.com/dashboard/integrations
  name: vdkApiKey
  revocation: A revoked key returns 401 and immediately deactivates every REST Hook subscription created with that key.
  scheme: bearer
  type: http
- applies_to: API-key management routes (GET/POST /keys, DELETE /keys/:id)
  description: Key management uses the customer's normal VeraDial session bearer token, not a vdk_ Zapier API key.
  name: sessionBearer
  scheme: bearer
  type: http
- applies_to: VeraDial MCP Server (https://api.veradial.com/mcp)
  description: OAuth 2.1 with the customer's existing VeraDial login; connector tokens are audience-bound to the MCP server and rejected elsewhere. No API keys.
  flows:
  - authorization_endpoint: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/authorize
    authorization_server: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registration_endpoint: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/clients/register
    token_endpoint: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/token
    token_endpoint_auth_methods:
    - none
  name: mcpOAuth
  protected_resource_metadata: https://api.veradial.com/.well-known/oauth-protected-resource
  type: oauth2
- applies_to: Custom signed event webhooks (outbound from VeraDial)
  description: X-VeraDial-Signature t=<unix-seconds>,v1=<hex digest>, HMAC-SHA256 over "<timestamp>.<raw body>" with the endpoint's whsec_ secret.
  docs: https://veradial.com/help/webhooks-make-n8n
  name: webhookSignature
  type: hmac
slug: veradial-authentication
source_filename: veradial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: searched\nsource:\n- https://veradial.com/help/zapier-integration-api\n- https://veradial.com/for-agents\n- https://api.veradial.com/.well-known/oauth-protected-resource\n- https://api.veradial.com/.well-known/oauth-authorization-server\ndocs: https://veradial.com/help/zapier-integration-api\nsummary:\n  types: [http-bearer, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: vdkApiKey\n  type: http\n  scheme: bearer\n  applies_to: VeraDial Zapier Integration API (hooks, lines, samples, me)\n  key_prefix: vdk_\n  description: 'Zapier-facing requests authenticate with Authorization: Bearer vdk_... using an API key generated\n    from the VeraDial Integrations dashboard. The key is a narrow credential: it works only with the hooks, lines,\n    samples, and me endpoints, and its full value is shown once. VeraDial Plus is required to create a key.'\n  management: https://app.veradial.com/dashboard/integrations\n\
  \  revocation: A revoked key returns 401 and immediately deactivates every REST Hook subscription created with that key.\n- name: sessionBearer\n  type: http\n  scheme: bearer\n  applies_to: API-key management routes (GET/POST /keys, DELETE /keys/:id)\n  description: Key management uses the customer's normal VeraDial session bearer token, not a vdk_ Zapier API key.\n- name: mcpOAuth\n  type: oauth2\n  applies_to: VeraDial MCP Server (https://api.veradial.com/mcp)\n  description: OAuth 2.1 with the customer's existing VeraDial login; connector tokens are audience-bound to the MCP\n    server and rejected elsewhere. No API keys.\n  flows:\n  - flow: authorizationCode\n    authorization_server: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1\n    authorization_endpoint: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/authorize\n    token_endpoint: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/token\n    registration_endpoint: https://rrmjstsbidgkqibvzvzo.supabase.co/auth/v1/oauth/clients/register\n\
  \    pkce: S256\n    token_endpoint_auth_methods: [none]\n    grant_types: [authorization_code, refresh_token]\n  protected_resource_metadata: https://api.veradial.com/.well-known/oauth-protected-resource\n- name: webhookSignature\n  type: hmac\n  applies_to: Custom signed event webhooks (outbound from VeraDial)\n  description: X-VeraDial-Signature t=<unix-seconds>,v1=<hex digest>, HMAC-SHA256 over \"<timestamp>.<raw body>\"\n    with the endpoint's whsec_ secret.\n  docs: https://veradial.com/help/webhooks-make-n8n\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veradial/refs/heads/main/authentication/veradial-authentication.yml
summary_line: http-bearer/oauth2 · 4 schemes
tags:
- AI Receptionist
- Business Phone
- Telephony
- Voice AI
- SMS
- Webhook
- MCP
- Small Business
---
