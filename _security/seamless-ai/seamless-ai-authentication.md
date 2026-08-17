---
api_key_in:
- header
api_specs:
- filename: seamless-ai-public-api-openapi-original.json
  format: json
  label: Seamless.AI Public API
  slug: seamless-ai-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/_original/seamless-ai-public-api-openapi-original.json
- filename: seamless-ai-mcp-server-openapi-original.yaml
  format: yaml
  label: Seamless.AI MCP Server
  slug: seamless-ai-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/_original/seamless-ai-mcp-server-openapi-original.yaml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Seamless Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Seamless.AI secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Seamless.AI
provider_slug: seamless-ai
scheme_count: 3
schemes:
- client_authentication: client_secret
  docs: https://docs.seamless.ai/authentication/oauth
  flows:
  - authorizationUrl: https://login.seamless.ai/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.seamless.ai/api/client/v1/oauth/accessToken
  name: OAuth2
  pkce: false
  real_scope: publicAPI.v1.all
  scope_note: 'The spec declares scopes: {} . The real scope, publicAPI.v1.all, is published only in prose. See scopes/seamless-ai-scopes.yml.'
  scopes_in_spec: 0
  sources:
  - openapi/seamless-ai-company-research-api-openapi.yml
  - openapi/seamless-ai-company-search-api-openapi.yml
  - openapi/seamless-ai-contact-research-api-openapi.yml
  - openapi/seamless-ai-contact-search-api-openapi.yml
  - openapi/seamless-ai-oauth-api-openapi.yml
  - openapi/seamless-ai-org-companies-api-openapi.yml
  - openapi/seamless-ai-org-contacts-api-openapi.yml
  token_response_fields:
  - access_token
  - refresh_token
  - expires_at
  type: oauth2
- also_valid_on_mcp: true
  created_at: https://login.seamless.ai/settings/public-api
  description: API key passed via the Token header.
  docs: https://docs.seamless.ai/authentication/api-keys
  header_value: the raw API key, with no scheme prefix
  in: header
  name: ApiKeyAuth
  parameter: Token
  sources:
  - openapi/seamless-ai-company-research-api-openapi.yml
  - openapi/seamless-ai-company-search-api-openapi.yml
  - openapi/seamless-ai-contact-research-api-openapi.yml
  - openapi/seamless-ai-contact-search-api-openapi.yml
  - openapi/seamless-ai-oauth-api-openapi.yml
  - openapi/seamless-ai-org-companies-api-openapi.yml
  - openapi/seamless-ai-org-contacts-api-openapi.yml
  type: apiKey
- description: Webhook secret that you can use to validate the request is originated by Seamless
  direction: inbound
  hmac: false
  in: header
  name: webhookSecret
  parameter: x-seamless-webhook-secret
  role: Shared secret Seamless.AI sends on webhook deliveries so the receiver can verify origin.
  see_also: asyncapi/seamless-ai-webhooks.yml
  sources:
  - openapi/seamless-ai-company-research-api-openapi.yml
  - openapi/seamless-ai-company-search-api-openapi.yml
  - openapi/seamless-ai-contact-research-api-openapi.yml
  - openapi/seamless-ai-contact-search-api-openapi.yml
  - openapi/seamless-ai-oauth-api-openapi.yml
  - openapi/seamless-ai-org-companies-api-openapi.yml
  - openapi/seamless-ai-org-contacts-api-openapi.yml
  type: apiKey
slug: seamless-ai-authentication
source_filename: seamless-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.seamless.ai/authentication/api-keys
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/seamless-ai-company-research-api-openapi.yml, openapi/seamless-ai-company-search-api-openapi.yml,\n  openapi/seamless-ai-contact-research-api-openapi.yml, openapi/seamless-ai-contact-search-api-openapi.yml,\n  openapi/seamless-ai-oauth-api-openapi.yml, openapi/seamless-ai-org-companies-api-openapi.yml, openapi/seamless-ai-org-contacts-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  oauth2_scopes:\n  - publicAPI.v1.all\n  - mcp.all\n  surfaces:\n  - rest\n  - mcp\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.seamless.ai/oauth/authorize\n    tokenUrl: https://api.seamless.ai/api/client/v1/oauth/accessToken\n    scopes: 0\n  sources:\n  - openapi/seamless-ai-company-research-api-openapi.yml\n  - openapi/seamless-ai-company-search-api-openapi.yml\n  - openapi/seamless-ai-contact-research-api-openapi.yml\n\
  \  - openapi/seamless-ai-contact-search-api-openapi.yml\n  - openapi/seamless-ai-oauth-api-openapi.yml\n  - openapi/seamless-ai-org-companies-api-openapi.yml\n  - openapi/seamless-ai-org-contacts-api-openapi.yml\n  docs: https://docs.seamless.ai/authentication/oauth\n  scopes_in_spec: 0\n  real_scope: publicAPI.v1.all\n  scope_note: 'The spec declares scopes: {} . The real scope, publicAPI.v1.all, is published only in prose.\n    See scopes/seamless-ai-scopes.yml.'\n  client_authentication: client_secret\n  pkce: false\n  token_response_fields:\n  - access_token\n  - refresh_token\n  - expires_at\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Token\n  description: API key passed via the Token header.\n  sources:\n  - openapi/seamless-ai-company-research-api-openapi.yml\n  - openapi/seamless-ai-company-search-api-openapi.yml\n  - openapi/seamless-ai-contact-research-api-openapi.yml\n  - openapi/seamless-ai-contact-search-api-openapi.yml\n  - openapi/seamless-ai-oauth-api-openapi.yml\n\
  \  - openapi/seamless-ai-org-companies-api-openapi.yml\n  - openapi/seamless-ai-org-contacts-api-openapi.yml\n  header_value: the raw API key, with no scheme prefix\n  created_at: https://login.seamless.ai/settings/public-api\n  docs: https://docs.seamless.ai/authentication/api-keys\n  also_valid_on_mcp: true\n- name: webhookSecret\n  type: apiKey\n  in: header\n  parameter: x-seamless-webhook-secret\n  description: Webhook secret that you can use to validate the request is originated by Seamless\n  sources:\n  - openapi/seamless-ai-company-research-api-openapi.yml\n  - openapi/seamless-ai-company-search-api-openapi.yml\n  - openapi/seamless-ai-contact-research-api-openapi.yml\n  - openapi/seamless-ai-contact-search-api-openapi.yml\n  - openapi/seamless-ai-oauth-api-openapi.yml\n  - openapi/seamless-ai-org-companies-api-openapi.yml\n  - openapi/seamless-ai-org-contacts-api-openapi.yml\n  direction: inbound\n  role: Shared secret Seamless.AI sends on webhook deliveries so the receiver can\
  \ verify origin.\n  hmac: false\n  see_also: asyncapi/seamless-ai-webhooks.yml\ndocs: https://docs.seamless.ai/authentication/api-keys\nsources:\n- https://docs.seamless.ai/authentication/api-keys\n- https://docs.seamless.ai/authentication/oauth\n- https://docs.seamless.ai/mcp/authentication\n- https://mcp.seamless.ai/.well-known/oauth-authorization-server\n- openapi/_original/seamless-ai-public-api-openapi-original.json\nnote: 'Upgraded from derived to searched against the provider''s own authentication pages. Seamless.AI\n  runs TWO independent auth surfaces: the REST Public API v1 (API key in a `Token` header, or OAuth 2.0\n  authorization-code with a client_secret against login.seamless.ai) and the MCP server (OAuth 2.1 with\n  PKCE S256, dynamic client registration, no client_secret, against mcp.seamless.ai). The same API key\n  also works on MCP. The docs warn explicitly that the API key header (`Token`) and the OAuth header (`Authorization:\n  Bearer`) must not be mixed on one request.\
  \ `webhookSecret` is not a caller credential -- it is the inbound\n  shared secret Seamless sends to YOUR endpoint on a webhook delivery.'\nmcp_authentication:\n  surface: https://mcp.seamless.ai/mcp\n  protocol: OAuth 2.1\n  authorization_endpoint: https://mcp.seamless.ai/mcp/authorize\n  token_endpoint: https://mcp.seamless.ai/mcp/token\n  registration_endpoint: https://mcp.seamless.ai/mcp/register\n  revocation_endpoint: https://mcp.seamless.ai/mcp/revoke\n  grant_types:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - none\n  dynamic_client_registration: true\n  scopes:\n  - mcp.all\n  discovery:\n  - /.well-known/oauth-authorization-server\n  - /.well-known/oauth-protected-resource\n  alternate: API key via the Token header\n  verified: Anonymous POST to https://mcp.seamless.ai/mcp returned HTTP 401 with a WWW-Authenticate Bearer\n    challenge carrying resource_metadata and scope=\"mcp.all\" (2026-08-14).\nentitlement_gate:\n\
  \  rest: HTTP 422 code=missingLicense when the org has no active Public API license.\n  mcp: '\"MCP Server access is not enabled for your account\"; per-domain tool visibility further filtered\n    by the Connect license.'\n  note: Authentication succeeding does not mean authorization succeeds. Both surfaces gate on a license\n    separate from the credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/authentication/seamless-ai-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- B2B
- Contact Data
- Sales Intelligence
- Prospecting
- Lead Generation
- CRM Enrichment
- Data Enrichment
- MCP
- Agents
- Sales Automation
---
