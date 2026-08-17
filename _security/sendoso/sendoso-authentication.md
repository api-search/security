---
api_key_in: []
api_specs:
- filename: sendoso-core-api-openapi.yml
  format: yaml
  label: Sendoso Core API
  slug: sendoso-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/openapi/sendoso-core-api-openapi.yml
- filename: sendoso-marketplace-api-openapi.yml
  format: yaml
  label: Sendoso Marketplace and SmartSend API
  slug: sendoso-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/openapi/sendoso-marketplace-api-openapi.yml
- filename: sendoso-scim-api-openapi.yml
  format: yaml
  label: Sendoso SCIM API
  slug: sendoso-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/openapi/sendoso-scim-api-openapi.yml
- filename: sendoso-webhooks-asyncapi.yml
  format: yaml
  label: Sendoso Webhooks
  slug: sendoso-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/asyncapi/sendoso-webhooks-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sendoso Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sendoso secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sendoso
provider_slug: sendoso
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Authorization Code grant. Register your application by contacting developers@sendoso.com to receive a client ID and client secret. Access tokens live 7200 seconds (2 hours) and are refreshed at the same token endpoint. Tokens are sent as `Authorization: Bearer <token>`.'
  flows:
  - authorizationUrl: https://app.sendoso.com/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://app.sendoso.com/oauth/token
  name: OAuth2
  sources:
  - openapi/sendoso-core-api-openapi.yml
  - openapi/sendoso-marketplace-api-openapi.yml
  - openapi/sendoso-scim-api-openapi.yml
  type: oauth2
slug: sendoso-authentication
source_filename: sendoso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.sendoso.com/rest-api/overview/authentication\ndocs:\n  - https://developer.sendoso.com/rest-api/overview/authentication\n  - https://developer.sendoso.com/scim/overview/authentication\n  - https://developer.sendoso.com/marketplace/overview/authentication\n  - https://developer.sendoso.com/rest-api/overview/security\nderived_from:\n  - openapi/sendoso-core-api-openapi.yml\n  - openapi/sendoso-marketplace-api-openapi.yml\n  - openapi/sendoso-scim-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.sendoso.com/oauth/authorize\n    tokenUrl: https://app.sendoso.com/oauth/token\n    scopes: 5\n  description: 'OAuth 2.0 Authorization Code grant. Register your application by contacting\n    developers@sendoso.com to receive a client ID and client secret. Access tokens\
  \ live 7200\n    seconds (2 hours) and are refreshed at the same token endpoint. Tokens are sent as `Authorization:\n    Bearer <token>`.'\n  sources:\n  - openapi/sendoso-core-api-openapi.yml\n  - openapi/sendoso-marketplace-api-openapi.yml\n  - openapi/sendoso-scim-api-openapi.yml\nregistration:\n  self_serve: false\n  process: >-\n    Client ID and client secret are issued by hand. Sendoso's docs say to request credentials\n    by emailing developers@sendoso.com, and to include your production redirect URI — by\n    default only the standard Postman redirect URI is allowlisted. SCIM requires a SEPARATE\n    client id and secret; Core API credentials do not work against the SCIM API.\n  contact: developers@sendoso.com\ntoken:\n  type: bearer\n  header: 'Authorization: Bearer <token>'\n  lifetime_seconds: 7200\n  refresh: >-\n    POST the same token endpoint with grant_type=refresh_token. Refresh tokens only expire\n    after they are used.\n  revocation_endpoint: https://app.sendoso.com/oauth/revoke\n\
  \  revocation_auth: 'Basic base64(client_id:client_secret)'\n  revocation_note: The token to revoke is passed as a `token` query parameter.\ntransport_security:\n  claim: >-\n    Sendoso's security page states data is encrypted at rest with AES-256 and in transit over\n    HTTPS TLS 1.2 with RSA 256-bit.\n  source: https://developer.sendoso.com/rest-api/overview/security\n  observed_tls: TLSv1.3 on app.sendoso.com, developer.sendoso.com and sendoso.com (probed 2026-08-13)\nadditional_authorization_servers:\n  - name: Sendoso MCP Server\n    resource: https://app.sendoso.com/mcp\n    issuer: https://app.sendoso.com/mcp\n    discovery:\n      protected_resource_metadata: https://app.sendoso.com/.well-known/oauth-protected-resource/mcp\n      authorization_server_metadata: https://app.sendoso.com/.well-known/oauth-authorization-server/mcp\n    grant_types: [authorization_code, refresh_token]\n    pkce: S256\n    dynamic_client_registration: https://app.sendoso.com/mcp/oauth/register\n   \
  \ scopes: [openid, profile, email, offline_access]\n    idp: Auth0 (jwks https://sendosoprod.auth0.com/.well-known/jwks.json)\n    note: >-\n      Separate from the developer API's OAuth server. This one supports OIDC scopes, PKCE and\n      dynamic client registration, none of which the developer API advertises — the MCP\n      surface is materially more modern than the REST surface it fronts.\nnotes:\n  - >-\n    Sendoso's own security page tells you to \"revoke your API key\" when finished, but the API\n    has no API keys — it is OAuth only. That sentence is a leftover.\n  - >-\n    The docs describe the authorization code grant as \"two-legged\" / \"two-step\" OAuth. That\n    is a misnomer; authorization code is three-legged.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendoso/refs/heads/main/authentication/sendoso-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Corporate Gifting
- Direct Mail
- Sales Engagement
- Marketing Automation
- CRM Integration
- eGifts
- Swag and Merchandise
- Fulfillment
- Employee Recognition
- Account Based Marketing
- SCIM Provisioning
- Webhooks
---
