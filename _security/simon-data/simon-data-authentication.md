---
api_key_in:
- body
api_specs:
- filename: simon-data-audience-api-openapi.yml
  format: yaml
  label: Simon Data Audience API
  slug: simon-data-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-audience-api-openapi.yml
- filename: simon-data-event-ingestion-openapi.yml
  format: yaml
  label: Simon Data Event Ingestion API
  slug: simon-data-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-event-ingestion-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Simon Data Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Simon Data secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Simon Data
provider_slug: simon-data
scheme_count: 3
schemes:
- api: Simon Data Audience API
  description: 'Bearer token issued by a Simon Data Client Solutions Manager, sent as `Authorization: Bearer <token>`. Tokens are requested, rotated and deleted through a support ticket; Simon documents that tokens must never be sent by email or Slack and should be referenced by their last three digits. Server-side use only — Simon explicitly recommends against calling the Audience API from client-side applications.'
  docs: https://docs.simondata.com/reference/getting-started
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/simon-data-audience-api-openapi.yml
  type: http
- api: Simon Data Event Ingestion API
  description: Shared secret carried in the event payload alongside partnerId, which identifies the customer's site. Both values are issued by Simon and shown in the app under Admin Center > Signal Installation. Because the secret travels in the body of a browser-originated collect call when Simon.JS is used, it is a site-scoped write credential, not a confidential server credential.
  docs: https://docs.simondata.com/reference/event-ingestion-api
  in: body
  name: partnerSecret
  parameter: partnerSecret
  sources:
  - openapi/simon-data-event-ingestion-openapi.yml
  type: apiKey
- api: Simon Data MCP surface
  description: OAuth 2.0 authorization-code flow with PKCE and dynamic client registration, published as RFC 8414 metadata at https://app.simondata.com/.well-known/oauth-authorization-server. No scopes are advertised in the metadata document.
  flows:
  - authorizationUrl: https://app.simondata.com/mcp/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://app.simondata.com/mcp/oauth/register
    scopes: 0
    tokenUrl: https://app.simondata.com/mcp/oauth/token
  name: mcp-oauth
  sources:
  - well-known/simon-data-oauth-authorization-server.json
  type: oauth2
slug: simon-data-authentication
source_filename: simon-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.simondata.com/reference/getting-started\ndocs: https://docs.simondata.com/reference/getting-started\nnote: >-\n  Upgraded from a derived profile that reported an oauth2 clientCredentials flow with a token URL of\n  https://api.simondata.com/oauth/token. That token URL appears nowhere in Simon Data's documentation and came from a\n  scaffolded spec, which has been removed. Simon Data's own OpenAPI on its ReadMe hub declares a placeholder oauth2\n  scheme with an empty flows object; the Getting Started page states plainly that the Audience API uses bearer-token\n  authentication with a token issued by a Client Solutions Manager. The Event Ingestion API does not use a header at\n  all — it authenticates with a shared partnerSecret carried inside the JSON payload.\nsummary:\n  types: [http, apiKey, oauth2]\n  api_key_in: [body]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: bearerAuth\n  type: http\n  scheme:\
  \ bearer\n  api: Simon Data Audience API\n  in: header\n  parameter: Authorization\n  description: >-\n    Bearer token issued by a Simon Data Client Solutions Manager, sent as `Authorization: Bearer <token>`. Tokens are\n    requested, rotated and deleted through a support ticket; Simon documents that tokens must never be sent by email or\n    Slack and should be referenced by their last three digits. Server-side use only — Simon explicitly recommends\n    against calling the Audience API from client-side applications.\n  docs: https://docs.simondata.com/reference/getting-started\n  sources: [openapi/simon-data-audience-api-openapi.yml]\n- name: partnerSecret\n  type: apiKey\n  in: body\n  parameter: partnerSecret\n  api: Simon Data Event Ingestion API\n  description: >-\n    Shared secret carried in the event payload alongside partnerId, which identifies the customer's site. Both values\n    are issued by Simon and shown in the app under Admin Center > Signal Installation. Because the\
  \ secret travels in the\n    body of a browser-originated collect call when Simon.JS is used, it is a site-scoped write credential, not a\n    confidential server credential.\n  docs: https://docs.simondata.com/reference/event-ingestion-api\n  sources: [openapi/simon-data-event-ingestion-openapi.yml]\n- name: mcp-oauth\n  type: oauth2\n  api: Simon Data MCP surface\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.simondata.com/mcp/oauth/authorize\n    tokenUrl: https://app.simondata.com/mcp/oauth/token\n    registrationUrl: https://app.simondata.com/mcp/oauth/register\n    pkce: S256\n    scopes: 0\n  description: >-\n    OAuth 2.0 authorization-code flow with PKCE and dynamic client registration, published as RFC 8414 metadata at\n    https://app.simondata.com/.well-known/oauth-authorization-server. No scopes are advertised in the metadata document.\n  sources: [well-known/simon-data-oauth-authorization-server.json]\noutbound:\n  note: >-\n    For outbound integrations\
  \ and webhooks Simon is the client, not the server. Simon supports OAuth2 on outbound\n    webhook destinations and will automatically re-authenticate and retry on 401, 403 or 419 responses.\n  docs: https://docs.simondata.com/reference/outbound-integration-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/authentication/simon-data-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Customer Data Platform
- CDP
- Marketing Automation
- Audience Segmentation
- Event Tracking
- Data Ingestion
- Personalization
- Marketing Technology
- Identity Resolution
- Customer Profiles
- Journey Orchestration
- Snowflake
---
