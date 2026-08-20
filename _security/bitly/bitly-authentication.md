---
api_key_in: []
api_specs:
- filename: bitly-bsds-api-openapi.yml
  format: yaml
  label: Bitly BSDs API
  slug: bitly-bsds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-bsds-api-openapi.yml
- filename: bitly-bitlinks-api-openapi.yml
  format: yaml
  label: Bitly Bitlinks API
  slug: bitly-bitlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-bitlinks-api-openapi.yml
- filename: bitly-campaigns-api-openapi.yml
  format: yaml
  label: Bitly Campaigns API
  slug: bitly-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-campaigns-api-openapi.yml
- filename: bitly-custom-bitlinks-api-openapi.yml
  format: yaml
  label: Bitly Custom Bitlinks API
  slug: bitly-custom-bitlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-custom-bitlinks-api-openapi.yml
- filename: bitly-groups-api-openapi.yml
  format: yaml
  label: Bitly Groups API
  slug: bitly-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-groups-api-openapi.yml
- filename: bitly-oauth-apps-api-openapi.yml
  format: yaml
  label: Bitly OAuth Apps API
  slug: bitly-oauth-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-oauth-apps-api-openapi.yml
- filename: bitly-organizations-api-openapi.yml
  format: yaml
  label: Bitly Organizations API
  slug: bitly-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-organizations-api-openapi.yml
- filename: bitly-qr-codes-api-openapi.yml
  format: yaml
  label: Bitly QR Codes API
  slug: bitly-qr-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-qr-codes-api-openapi.yml
- filename: bitly-user-api-openapi.yml
  format: yaml
  label: Bitly User API
  slug: bitly-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-user-api-openapi.yml
- filename: bitly-webhooks-api-openapi.yml
  format: yaml
  label: Bitly Webhooks API
  slug: bitly-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/openapi/bitly-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Bitly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitly secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bitly
provider_slug: bitly
scheme_count: 2
schemes:
- description: A generic access token generated from Bitly account Developer settings. This is the path Bitly's docs recommend for point-to-point integrations and is what the MCP quickstart uses.
  format: 'Authorization: Bearer {token}'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/bitly-v4-openapi.json
  token_source: https://bitly.com/settings/api
  type: http
- app_registration: Log in to Bitly, open Developer settings and click "Register new app"; a client_id and client_secret are issued after email confirmation.
  code_challenge_methods_supported:
  - S256
  description: Used to act on behalf of an end user so that shortened links land in that user's own Bitly history. Not declared in Bitly's OpenAPI; documented in the auth guide and advertised in RFC 8414 metadata on the API host.
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://bitly.com/oauth/authorize
      scopes: {}
      tokenUrl: https://api-ssl.bitly.com/oauth/access_token
  grant_types_supported:
  - authorization_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://bitly.com
  jwks_uri: https://api-ssl.bitly.com/.well-known/jwks.json
  name: oauth2
  registration_endpoint: https://api-ssl.bitly.com/oauth/register
  response_types_supported:
  - code
  sources:
  - https://dev.bitly.com/docs/getting-started/authentication
  - well-known/bitly-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - none
  type: oauth2
slug: bitly-authentication
source_filename: bitly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://dev.bitly.com/docs/getting-started/authentication (docs), enriched over the derived\n  baseline from openapi/_original/bitly-v4-openapi.json and the live RFC 8414 metadata at\n  https://api-ssl.bitly.com/.well-known/oauth-authorization-server\ndocs: https://dev.bitly.com/docs/getting-started/authentication\nsummary:\n  types: [http, oauth2]\n  primary: bearer token\n  scopes_published: false\n  note: >-\n    Bitly's OpenAPI declares only a single `bearerAuth` HTTP bearer scheme. That understates the\n    real posture: Bitly also runs a full OAuth 2.0 authorization server, discoverable at\n    /.well-known/oauth-authorization-server on the API host, which is what the MCP server\n    authenticates against. The spec never models it, so a spec-only read of Bitly's auth is\n    wrong. No scopes are defined anywhere — tokens carry the full permissions of the granting\n    user and group.\nschemes:\n- name: bearerAuth\n\
  \  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer {token}'\n  description: >-\n    A generic access token generated from Bitly account Developer settings. This is the path\n    Bitly's docs recommend for point-to-point integrations and is what the MCP quickstart uses.\n  token_source: https://bitly.com/settings/api\n  sources: [openapi/_original/bitly-v4-openapi.json]\n- name: oauth2\n  type: oauth2\n  description: >-\n    Used to act on behalf of an end user so that shortened links land in that user's own Bitly\n    history. Not declared in Bitly's OpenAPI; documented in the auth guide and advertised in\n    RFC 8414 metadata on the API host.\n  issuer: https://bitly.com\n  flows:\n    authorizationCode:\n      authorizationUrl: https://bitly.com/oauth/authorize\n      tokenUrl: https://api-ssl.bitly.com/oauth/access_token\n      scopes: {}\n  registration_endpoint: https://api-ssl.bitly.com/oauth/register\n  jwks_uri: https://api-ssl.bitly.com/.well-known/jwks.json\n\
  \  grant_types_supported: [authorization_code]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, none]\n  id_token_signing_alg_values_supported: [RS256]\n  dynamic_client_registration: true\n  app_registration: >-\n    Log in to Bitly, open Developer settings and click \"Register new app\"; a client_id and\n    client_secret are issued after email confirmation.\n  sources:\n  - https://dev.bitly.com/docs/getting-started/authentication\n  - well-known/bitly-oauth-authorization-server.json\nlegacy_flows:\n- name: Resource Owner Credentials Grant\n  status: documented\n  note: >-\n    POST username+password to /oauth/access_token with HTTP Basic credentials. Bitly still\n    documents it; it is a deprecated pattern in OAuth 2.1 and should not be used for new work.\n- name: HTTP Basic Authentication\n  status: documented\n  note: >-\n    Single-call token retrieval intended for\
  \ command-line scripts. Accounts with two-factor\n    authentication cannot use it — Bitly returns `2FA_CODE_REQUESTED` and requires a second\n    request carrying an SMS code.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/authentication/bitly-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Links
- URL Shortener
- QR Codes
- Analytics
- Marketing
- Link Management
- Webhook
- Attribution
- Agents
- MCP
---
