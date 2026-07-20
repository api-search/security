---
api_key_in: []
api_specs:
- filename: kiteworks-core-openapi-original.json
  format: json
  label: Kiteworks Core API
  slug: core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kiteworks/refs/heads/main/openapi/kiteworks-core-openapi-original.json
- filename: kiteworks-pubsub-openapi-original.yml
  format: yaml
  label: Kiteworks PubSub Consumer API
  slug: pubsub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kiteworks/refs/heads/main/openapi/kiteworks-pubsub-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Kiteworks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- jwt-bearer
overview: Kiteworks secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and jwt-bearer flow(s).
provider_name: Kiteworks
provider_slug: kiteworks
scheme_count: 2
schemes:
- authorizationUrl: https://{kiteworks_server}/oauth/authorize
  flow: authorizationCode
  grant_type: authorization_code
  name: OAuth2AuthorizationCode
  pkce: Strongly recommended; required for public clients (mobile apps, SPAs)
  purpose: Interactive user sign-in for web, desktop and mobile applications.
  request_params:
  - client_id
  - client_secret
  - redirect_uri
  - scope
  - response_type=code
  - state (optional)
  - m=1 (optional, mobile-friendly UI)
  response_fields:
  - access_token
  - expires_in
  - token_type (always "bearer")
  - scope
  - refresh_token (when configured)
  tokenUrl: https://{kiteworks_server}/oauth/token
  type: oauth2
- flow: jwt-bearer
  grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
  jwt_claims:
  - iss (issuer)
  - sub (Kiteworks user email)
  - aud (audience)
  - iat
  - nbf
  - exp (typically 5 minutes)
  - jti (unique id, replay prevention)
  name: OAuth2JWTBearer
  purpose: Backend automation, scheduled jobs and unattended scripts; server-side user impersonation.
  refresh_token: false
  response_fields:
  - access_token
  - expires_in
  - token_type
  - scope
  signing: RS256 by default (RSA key pair generated with OpenSSL; public key registered in the Admin console)
  tokenUrl: https://{kiteworks_server}/oauth/token
  type: oauth2
slug: kiteworks-authentication
source_filename: kiteworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.kiteworks.com/authentication.html\ndocs: https://developer.kiteworks.com/authentication.html\nnote: The published v28 OpenAPI declares no components.securitySchemes, so this profile is taken from\n  the developer portal authentication guide rather than derived from the spec. Endpoints are per-tenant\n  against the customer Kiteworks appliance.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - jwt-bearer\n  token_header: 'Authorization: Bearer <access_token>'\nprerequisites:\n- 'Enterprise package with the Developer Suite add-on enabled (Admin console: Application Setup -> Licenses,\n  API row must show \"Enabled\")'\n- A registered custom application providing client_id, client_secret, permitted scopes, redirect URIs\n  and token lifetimes\nschemes:\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://{kiteworks_server}/oauth/authorize\n\
  \  tokenUrl: https://{kiteworks_server}/oauth/token\n  grant_type: authorization_code\n  pkce: Strongly recommended; required for public clients (mobile apps, SPAs)\n  purpose: Interactive user sign-in for web, desktop and mobile applications.\n  request_params:\n  - client_id\n  - client_secret\n  - redirect_uri\n  - scope\n  - response_type=code\n  - state (optional)\n  - m=1 (optional, mobile-friendly UI)\n  response_fields:\n  - access_token\n  - expires_in\n  - token_type (always \"bearer\")\n  - scope\n  - refresh_token (when configured)\n- name: OAuth2JWTBearer\n  type: oauth2\n  flow: jwt-bearer\n  tokenUrl: https://{kiteworks_server}/oauth/token\n  grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n  purpose: Backend automation, scheduled jobs and unattended scripts; server-side user impersonation.\n  signing: RS256 by default (RSA key pair generated with OpenSSL; public key registered in the Admin console)\n  jwt_claims:\n  - iss (issuer)\n  - sub (Kiteworks user email)\n\
  \  - aud (audience)\n  - iat\n  - nbf\n  - exp (typically 5 minutes)\n  - jti (unique id, replay prevention)\n  response_fields:\n  - access_token\n  - expires_in\n  - token_type\n  - scope\n  refresh_token: false\napi_keys:\n  supported: false\n  evidence: The authentication guide documents OAuth 2.0 only; no API key scheme is offered.\nmcp_auth:\n  protocol: OAuth 2.1\n  dynamic_client_registration: true\n  pkce: true\n  note: The Kiteworks MCP Server (remote HTTPS mode) authenticates with OAuth 2.1 including Dynamic Client\n    Registration; see mcp/kiteworks-mcp.yml.\nsee:\n- scopes/kiteworks-scopes.yml\n- conventions/kiteworks-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiteworks/refs/heads/main/authentication/kiteworks-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Secure File Sharing
- Managed File Transfer
- Secure Email
- Data Governance
- Regulatory Compliance
- Content Security
- Private Data Network
- CMMC
- SCIM
---
