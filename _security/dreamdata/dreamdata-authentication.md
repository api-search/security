---
api_key_in:
- header
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Dreamdata Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Dreamdata secures its APIs with http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Dreamdata
provider_slug: dreamdata
scheme_count: 4
schemes:
- applies_to: Event Tracking API (https://api.dreamdata.cloud/v1/batch)
  description: HTTP Basic auth carrying the source API key as the username with an empty password, base64-encoded as "apiKey:". Used for server-side batch event submission.
  docs: https://developer.dreamdata.io/server-side/server-side-tracking/
  name: TrackingApiKeyBasic
  scheme: basic
  type: http
- applies_to: MCP server (https://mcp.dreamdata.io/mcp)
  authorization_endpoint: https://authenticate.dreamdata.io/oauth/2.1/authorize
  docs: https://developer.dreamdata.io/mcp/mcp-server/
  introspection_endpoint: https://authenticate.dreamdata.io/oauth/2.1/introspect
  name: MCPOAuth21
  pkce: S256
  registration_endpoint: https://authenticate.dreamdata.io/oauth/2.1/register
  scheme: authorizationCode+PKCE
  scopes:
  - read
  - reports:write
  token_endpoint: https://authenticate.dreamdata.io/oauth/2.1/token
  type: oauth2
- id_token_signing: RS256
  issuer: https://authenticate.dreamdata.io
  name: OpenIDConnect
  note: PropelAuth-backed OIDC used for app/console sign-in.
  openid_configuration: https://authenticate.dreamdata.io/.well-known/openid-configuration
  scopes:
  - openid
  - email
  - profile
  type: openIdConnect
- algorithm: HMAC-SHA256
  applies_to: Outbound audience webhook syncs
  description: Dreamdata appends an HMAC-SHA256 signature to outbound webhook sync requests; the signing key is retrievable per webhook sync so recipients can verify authenticity.
  docs: https://docs.dreamdata.io/article/mdebkprrgi-webhook-syncs
  name: WebhookHMAC
  type: signature
slug: dreamdata-authentication
source_filename: dreamdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.dreamdata.io/server-side/server-side-tracking/ + https://developer.dreamdata.io/mcp/mcp-server/\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: TrackingApiKeyBasic\n  type: http\n  scheme: basic\n  applies_to: Event Tracking API (https://api.dreamdata.cloud/v1/batch)\n  description: >-\n    HTTP Basic auth carrying the source API key as the username with an empty password,\n    base64-encoded as \"apiKey:\". Used for server-side batch event submission.\n  docs: https://developer.dreamdata.io/server-side/server-side-tracking/\n- name: MCPOAuth21\n  type: oauth2\n  scheme: authorizationCode+PKCE\n  pkce: S256\n  applies_to: MCP server (https://mcp.dreamdata.io/mcp)\n  authorization_endpoint: https://authenticate.dreamdata.io/oauth/2.1/authorize\n  token_endpoint: https://authenticate.dreamdata.io/oauth/2.1/token\n\
  \  introspection_endpoint: https://authenticate.dreamdata.io/oauth/2.1/introspect\n  registration_endpoint: https://authenticate.dreamdata.io/oauth/2.1/register\n  scopes:\n  - read\n  - reports:write\n  docs: https://developer.dreamdata.io/mcp/mcp-server/\n- name: OpenIDConnect\n  type: openIdConnect\n  issuer: https://authenticate.dreamdata.io\n  openid_configuration: https://authenticate.dreamdata.io/.well-known/openid-configuration\n  id_token_signing: RS256\n  scopes:\n  - openid\n  - email\n  - profile\n  note: PropelAuth-backed OIDC used for app/console sign-in.\n- name: WebhookHMAC\n  type: signature\n  algorithm: HMAC-SHA256\n  applies_to: Outbound audience webhook syncs\n  description: >-\n    Dreamdata appends an HMAC-SHA256 signature to outbound webhook sync requests; the\n    signing key is retrievable per webhook sync so recipients can verify authenticity.\n  docs: https://docs.dreamdata.io/article/mdebkprrgi-webhook-syncs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dreamdata/refs/heads/main/authentication/dreamdata-authentication.yml
summary_line: http/oauth2/openIdConnect · 4 schemes
tags:
- Company
- B2B Attribution
- Revenue Attribution
- Marketing Analytics
- Customer Journey
- Event Tracking
- Audience Activation
- Analytics
- MCP
---
