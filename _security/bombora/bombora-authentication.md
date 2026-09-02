---
api_key_in: []
api_specs:
- filename: bombora-intent-api-openapi.yml
  format: yaml
  label: Bombora Intent API
  slug: bombora-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-intent-api-openapi.yml
- filename: bombora-accountlists-api-openapi.yml
  format: yaml
  label: Bombora Account Lists API
  slug: bombora-accountlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-accountlists-api-openapi.yml
- filename: bombora-accounts-api-openapi.yml
  format: yaml
  label: Bombora Accounts API
  slug: bombora-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-accounts-api-openapi.yml
- filename: bombora-activate-api-openapi.yml
  format: yaml
  label: Bombora Activate API
  slug: bombora-activate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-activate-api-openapi.yml
- filename: bombora-data-api-openapi.yml
  format: yaml
  label: Bombora Data API
  slug: bombora-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-data-api-openapi.yml
- filename: bombora-demographic-api-openapi.yml
  format: yaml
  label: Bombora Demographic API
  slug: bombora-demographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-demographic-api-openapi.yml
- filename: bombora-destinations-api-openapi.yml
  format: yaml
  label: Bombora Destinations API
  slug: bombora-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-destinations-api-openapi.yml
- filename: bombora-digital-audience-builder-dab-api-api-openapi.yml
  format: yaml
  label: Bombora Digital Audience Builder (DAB) API
  slug: bombora-digital-audience-builder-dab-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-digital-audience-builder-dab-api-api-openapi.yml
- filename: bombora-estimate-api-openapi.yml
  format: yaml
  label: Bombora Estimate API
  slug: bombora-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-estimate-api-openapi.yml
- filename: bombora-events-api-openapi.yml
  format: yaml
  label: Bombora Events API
  slug: bombora-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-events-api-openapi.yml
- filename: bombora-firmographic-api-openapi.yml
  format: yaml
  label: Bombora Firmographic API
  slug: bombora-firmographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-firmographic-api-openapi.yml
- filename: bombora-geographic-api-openapi.yml
  format: yaml
  label: Bombora Geographic API
  slug: bombora-geographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-geographic-api-openapi.yml
- filename: bombora-install-data-api-openapi.yml
  format: yaml
  label: Bombora Install Data API
  slug: bombora-install-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-install-data-api-openapi.yml
- filename: bombora-oauth-api-openapi.yml
  format: yaml
  label: Bombora OAUTH API
  slug: bombora-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-oauth-api-openapi.yml
- filename: bombora-signaldefinition-api-openapi.yml
  format: yaml
  label: Bombora Signal Definition API
  slug: bombora-signaldefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-signaldefinition-api-openapi.yml
- filename: bombora-suspend-api-openapi.yml
  format: yaml
  label: Bombora Suspend API
  slug: bombora-suspend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/openapi/bombora-suspend-api-openapi.yml
auth_types:
- http
- oauth2-client-credentials
description: ''
kind: authentication
layout: security
method: searched
name: Bombora Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bombora secures its APIs with http and oauth2-client-credentials across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bombora
provider_slug: bombora
scheme_count: 1
schemes:
- applied: 'global (security: [{bearerAuth: []}]) on all five product APIs'
  bearerFormat: JWT
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/bombora-account-list-api-openapi.yml
  - openapi/bombora-digital-audience-api-openapi.yml
  - openapi/bombora-intent-api-openapi.yml
  - openapi/bombora-reference-api-openapi.yml
  - openapi/bombora-webhooks-api-openapi.yml
  type: http
slug: bombora-authentication
source_filename: bombora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  openapi/ (6 OpenAPI 3.0 documents), https://developer.bombora.com/get-started,\n  https://developer.bombora.com/docs/authentication-api/1/overview,\n  https://bombora-partners.atlassian.net/wiki/spaces/DOC/pages/1212420/Bombora+API\ndocs: https://developer.bombora.com/get-started\nsummary:\n  types: [http, oauth2-client-credentials]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  oauth2_flows_note: >-\n    The client-credentials exchange is real and documented on the Get Started page, but it is NOT\n    modelled as an oauth2 securityScheme in any spec — the five product specs declare only\n    bearerAuth (http/bearer/JWT) and the Authentication API spec declares no securityScheme at\n    all. There is consequently no scope map anywhere, so no scopes/ artifact is emitted.\n  scopes: 0\n  self_service: false\n\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter:\
  \ Authorization\n  applied: 'global (security: [{bearerAuth: []}]) on all five product APIs'\n  sources:\n  - openapi/bombora-account-list-api-openapi.yml\n  - openapi/bombora-digital-audience-api-openapi.yml\n  - openapi/bombora-intent-api-openapi.yml\n  - openapi/bombora-reference-api-openapi.yml\n  - openapi/bombora-webhooks-api-openapi.yml\n\ntoken_endpoint:\n  url: https://api.bombora.com/oauth/token\n  method: POST\n  api: Authentication API\n  spec: openapi/bombora-authentication-api-openapi.yml\n  docs: https://developer.bombora.com/docs/authentication-api/1/overview\n  credentials: ClientId (key) + ClientSecret (secret), issued per app in the developer portal\n  note: >-\n    \"The Authentication API must be enabled for your app otherwise calls to the /oauth/token\n    endpoint will fail.\" — developer.bombora.com/get-started\n\ncredential_issuance:\n  self_service: false\n  steps:\n  - Sign in to https://developer.bombora.com — the only sign-in option is LOGIN WITH SAML.\n  -\
  \ >-\n      You must already be a Bombora user; Bombora Support must associate your account with your\n      organisation's developer team before any team or app is visible.\n  - Select My Apps, open your developer team, then open your application under Apps.\n  - Read the ClientId (key) and ClientSecret (secret) from the app's API Keys section.\n  - >-\n      Request access to the API products you need; new applications require Bombora Support\n      approval before they work.\n  support: https://bombora.com/customer-support-forms/\n  api_products:\n  - {name: Reference API, approval: auto}\n  - {name: Authentication API, approval: auto}\n  - {name: Account List API, approval: auto}\n  - {name: Webhooks API, approval: auto}\n  - {name: Intent API, approval: manual}\n  - {name: Digital Audience API, approval: manual}\n  api_products_source: >-\n    https://developer.bombora.com/portals/api/sites/astute-harbor-103715-developerportalbombora/liveportal/apis\n\nlegacy_partner_auth:\n  api:\
  \ Company Surge API (v4)\n  host: https://sentry.bombora.com\n  type: http\n  scheme: basic\n  detail: >-\n    \"authorization key which will be a base 64 encoded string of username and password in the\n    format of username:password\" — the partner Confluence documentation. This is a different\n    credential from the portal's ClientId/ClientSecret and a different host; it is not covered by\n    any OpenAPI document.\n  docs: https://bombora-partners.atlassian.net/wiki/spaces/DOC/pages/1212420/Bombora+API\n\nunrelated_oauth_surface:\n  host: bombora.com\n  issuer: https://bombora.com\n  metadata: https://bombora.com/.well-known/oauth-authorization-server\n  scopes_supported: [mcp]\n  note: >-\n    The RFC 8414 document on bombora.com belongs to the WordPress MCP adapter on the marketing\n    site, not to the product APIs. Do not send its tokens to api.bombora.com. See\n    mcp/bombora-mcp.yml and well-known/bombora-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/authentication/bombora-authentication.yml
summary_line: http/oauth2-client-credentials · 1 scheme
tags:
- Intent Data
- B2B Intent
- Company Surge
- Account Based Marketing
- Sales Intelligence
- Marketing Intelligence
- Identity Resolution
- Audience Activation
- Data Cooperative
- Webhook
- Reference Data
- AdTech
- MarTech
- B2B
- Account Lists
- Digital Audience Builder
- OpenAPI
---
