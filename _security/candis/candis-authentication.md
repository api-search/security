---
api_key_in: []
api_specs:
- filename: candis-openapi.json
  format: json
  label: Candis API
  slug: candis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/openapi/candis-openapi.json
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Candis Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- tokenExchange
overview: Candis secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and tokenExchange flow(s).
provider_name: Candis
provider_slug: candis
scheme_count: 2
schemes:
- client_authentication: HTTP Basic (client_id:client_secret, base64-encoded)
  flows:
  - authorizationUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/auth
    flow: authorizationCode
    notes: User is redirected to consent and select an organization; authorization code is short-lived (expires in ~30-50 seconds) and exchanged for access + refresh tokens. Redirect URIs must be whitelisted by Candis. Desktop/limited-webserver clients use the out-of-band redirect https://my.candis.io/authentication_code.
    tokenUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token
  - flow: clientCredentials
    notes: Supported by the authorization server for service accounts (service_account scope).
    tokenUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token
  - docs: https://developer.candis.io/docs/token-exchange
    flow: tokenExchange
    grant_type: urn:ietf:params:oauth:grant-type:token-exchange
    tokenUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token
  grant_types_supported:
  - authorization_code
  - client_credentials
  - implicit
  - password
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:uma-ticket
  - urn:openid:params:grant-type:ciba
  identity_provider: Keycloak
  issuer: https://id.my.candis.io/auth/realms/candis
  name: oauth2
  sources:
  - https://developer.candis.io/docs/how-to-authenticate
  - well-known/candis-openid-configuration.json
  token_lifetimes:
    access_token_seconds_example: 1209600
    offline_access: Including the offline_access scope yields long-lived tokens (validity up to ~6-24 months) for background/long-running services.
    refresh_token_seconds_example: 15551995
  type: oauth2
- applies_to: https://api.candis.io/v1/organizations/*
  name: bearerAuth
  notes: 'All Candis resource API requests carry the OAuth access token as an "Authorization: Bearer {access_token}" header.'
  scheme: bearer
  sources:
  - openapi/candis-openapi.json
  type: http
slug: candis-authentication
source_filename: candis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.candis.io/docs/how-to-authenticate\ndocs:\n- https://developer.candis.io/docs/authentication-overview\n- https://developer.candis.io/docs/how-to-authenticate\n- https://developer.candis.io/docs/token-exchange\n- https://developer.candis.io/docs/access-token-scopes\noidc_discovery: https://id.my.candis.io/auth/realms/candis/.well-known/openid-configuration\nsummary:\n  types: [oauth2, openIdConnect]\n  primary: oauth2\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, tokenExchange]\n  token_transport: Authorization Bearer header\n  authorization_server: Keycloak (realm \"candis\")\nschemes:\n- name: oauth2\n  type: oauth2\n  identity_provider: Keycloak\n  issuer: https://id.my.candis.io/auth/realms/candis\n  client_authentication: HTTP Basic (client_id:client_secret, base64-encoded)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/auth\n\
  \    tokenUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token\n    notes: >-\n      User is redirected to consent and select an organization; authorization code is\n      short-lived (expires in ~30-50 seconds) and exchanged for access + refresh tokens.\n      Redirect URIs must be whitelisted by Candis. Desktop/limited-webserver clients use\n      the out-of-band redirect https://my.candis.io/authentication_code.\n  - flow: clientCredentials\n    tokenUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token\n    notes: Supported by the authorization server for service accounts (service_account scope).\n  - flow: tokenExchange\n    grant_type: urn:ietf:params:oauth:grant-type:token-exchange\n    tokenUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token\n    docs: https://developer.candis.io/docs/token-exchange\n  token_lifetimes:\n    access_token_seconds_example: 1209600\n    refresh_token_seconds_example: 15551995\n\
  \    offline_access: >-\n      Including the offline_access scope yields long-lived tokens (validity up to ~6-24\n      months) for background/long-running services.\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - urn:openid:params:grant-type:ciba\n  sources:\n  - https://developer.candis.io/docs/how-to-authenticate\n  - well-known/candis-openid-configuration.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  applies_to: https://api.candis.io/v1/organizations/*\n  notes: >-\n    All Candis resource API requests carry the OAuth access token as an\n    \"Authorization: Bearer {access_token}\" header.\n  sources:\n  - openapi/candis-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/authentication/candis-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Fintech
- Accounts Payable
- Spend Management
- Invoice Management
- Financial Process Automation
- Accounting
- DATEV
- OCR
- Germany
---
