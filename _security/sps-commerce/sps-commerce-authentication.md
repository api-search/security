---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sps-commerce-submission-api-openapi.yml
  format: yaml
  label: SPS Commerce Trading Partner Submission API
  slug: sps-commerce-trading-partner-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sps-commerce/refs/heads/main/openapi/sps-commerce-submission-api-openapi.yml
- filename: sps-commerce-inventory-api-openapi.yml
  format: yaml
  label: SPS Commerce Inventory API
  slug: sps-commerce-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sps-commerce/refs/heads/main/openapi/sps-commerce-inventory-api-openapi.yml
- filename: sps-commerce-import-api-openapi.yml
  format: yaml
  label: SPS Commerce Import API
  slug: sps-commerce-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sps-commerce/refs/heads/main/openapi/sps-commerce-import-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Sps Commerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: SPS Commerce secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SPS Commerce
provider_slug: sps-commerce
scheme_count: 3
schemes:
- description: 'Bearer authentication specify''s a bearer token in the ''Authorization'' header following the format:

    Authorization: Bearer <token>'
  name: SpsBearer
  scheme: bearer
  sources:
  - openapi/sps-commerce-inventory-api-openapi.yml
  - openapi/sps-commerce-submission-api-openapi.yml
  type: http
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/sps-commerce-submission-api-openapi.yml
  type: http
- application_types:
  - Web Service Applications (partners should use this type)
  - Native Applications (authorization code with code verifier / code challenge, PKCE)
  - Single Page Applications (implicit flow deprecated; must migrate to Authorization Code Flow with PKCE using the Auth0 SPA SDK by July 1st, 2026)
  - Machine-to-Machine Applications (Client Credentials Grant)
  credentials: App ID and App Secret per Dev Center application; separate Sandbox Keys and Production Keys
  description: The SPS Dev Center follows the OAuth 2.0 industry standard to allow secure authorization in a simple and standard way.
  flows:
    authorizationCode:
      authorize_endpoint: GET /authorize
      pkce: required for Native and Single Page Applications
      redirect_uri: must exactly match a redirect URL registered for the Dev Center app (mismatch returns 403)
    clientCredentials:
      audience: https://spscommerce.com
      legacy_audience: api://api.spscommerce.com/
      parameters:
      - audience
      - client_id
      - client_secret
      - grant_type
      token_endpoint: POST /oauth/token
  name: Dev Center OAuth 2.0
  refresh_tokens: Refresh Tokens enable you to get a new Access Token when the current one has expired. Since they don't expire, handle and store them with great care so they are not compromised.
  source: https://developercenter.spscommerce.com/#/docs/new-authentication-docs/machine2machine-applications
  token_check: GET /auth-check returns 204 No Content for a valid bearer token
  type: oauth2
slug: sps-commerce-authentication
source_filename: sps-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://developercenter.spscommerce.com/#/docs/new-authentication-docs/getting-an-access-token\ndocs: https://developercenter.spscommerce.com/#/docs/authentication\ndocs_pages:\n- https://developercenter.spscommerce.com/#/docs/authentication\n- https://developercenter.spscommerce.com/#/docs/new-authentication-docs/getting-an-access-token\n- https://developercenter.spscommerce.com/#/docs/new-authentication-docs/machine2machine-applications\n- https://developercenter.spscommerce.com/#/docs/new-authentication-docs/using-an-access-token\n- https://developercenter.spscommerce.com/#/docs/new-authentication-docs/refresh-tokens\n- https://developercenter.spscommerce.com/#/docs/new-authentication-docs/authentication-keys\n- https://developercenter.spscommerce.com/#/docs/new-authentication-docs/troubleshooting-common-issues\n- https://developercenter.spscommerce.com/#/docs/new-authentication-docs/client-updates-for-enhanced-security\n\
  summary:\n  types:\n  - http\n  - oauth2\n  note: The OpenAPI contracts declare only HTTP bearer; the Dev Center docs state \"Dev Center follows standard OAuth protocols for authenticating and authorizing API requests.\" Bearer tokens are OAuth 2.0 access tokens issued per Dev Center application.\nschemes:\n- name: SpsBearer\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer authentication specify's a bearer token in the 'Authorization' header following the format:\n    Authorization: Bearer <token>\n  sources:\n  - openapi/sps-commerce-inventory-api-openapi.yml\n  - openapi/sps-commerce-submission-api-openapi.yml\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/sps-commerce-submission-api-openapi.yml\n- name: Dev Center OAuth 2.0\n  type: oauth2\n  description: \"The SPS Dev Center follows the OAuth 2.0 industry standard to allow secure authorization in a simple and standard way.\"\n  application_types:\n  - Web Service Applications (partners should\
  \ use this type)\n  - Native Applications (authorization code with code verifier / code challenge, PKCE)\n  - Single Page Applications (implicit flow deprecated; must migrate to Authorization Code Flow with PKCE using the Auth0 SPA SDK by July 1st, 2026)\n  - Machine-to-Machine Applications (Client Credentials Grant)\n  flows:\n    clientCredentials:\n      token_endpoint: POST /oauth/token\n      parameters: [audience, client_id, client_secret, grant_type]\n      audience: https://spscommerce.com\n      legacy_audience: api://api.spscommerce.com/\n    authorizationCode:\n      authorize_endpoint: GET /authorize\n      redirect_uri: must exactly match a redirect URL registered for the Dev Center app (mismatch returns 403)\n      pkce: required for Native and Single Page Applications\n  refresh_tokens: \"Refresh Tokens enable you to get a new Access Token when the current one has expired. Since they don't expire, handle and store them with great care so they are not compromised.\"\n  token_check:\
  \ GET /auth-check returns 204 No Content for a valid bearer token\n  credentials: App ID and App Secret per Dev Center application; separate Sandbox Keys and Production Keys\n  source: https://developercenter.spscommerce.com/#/docs/new-authentication-docs/machine2machine-applications\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sps-commerce/refs/heads/main/authentication/sps-commerce-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- EDI
- Retail
- Supply Chain
- Commerce
- Trading Partners
- API Standards
---
