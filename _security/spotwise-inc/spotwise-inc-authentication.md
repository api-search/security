---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Spotwise Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spotwise, Inc. declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Spotwise, Inc.
provider_slug: spotwise-inc
scheme_count: 3
schemes:
- applies_to:
  - https://spotwise.ai/api/mcp
  - https://spotwise.ai/api (Payload CMS admin/write surface)
  bearer_methods_supported:
  - header
  flows:
    authorization_code:
      authorization_url: https://spotwise.ai/api/auth/oauth2/authorize
      pkce: required-capable — code_challenge_methods_supported [S256]
      refresh_url: https://spotwise.ai/api/auth/oauth2/token
      scopes:
        email: email address claim
        mcp:content.read: read the site's Payload CMS content collections over MCP
        mcp:content.write: write the site's Payload CMS content collections over MCP
        offline_access: refresh-token issuance
        openid: OpenID Connect identity
        profile: basic profile claims
      token_url: https://spotwise.ai/api/auth/oauth2/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: spotwise_oauth2
  issuer: https://spotwise.ai/api/auth
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
- applies_to:
  - https://app.spotwise.ai/api/mcp
  - https://app.spotwise.ai (product application)
  bearer_methods_supported:
  - header
  flows:
    authorization_code:
      authorization_url: https://app.spotwise.ai/api/auth/oauth2/authorize
      pkce: required-capable — code_challenge_methods_supported [S256]
      refresh_url: https://app.spotwise.ai/api/auth/oauth2/token
      scopes:
        email: email address claim
        offline_access: refresh-token issuance
        openid: OpenID Connect identity
        profile: basic profile claims
      token_url: https://app.spotwise.ai/api/auth/oauth2/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: spotwise_app_oauth2
  issuer: https://app.spotwise.ai/api/auth
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
- applies_to:
  - https://spotwise.ai/api (Payload CMS public READ surface)
  id: spotwise_none
  note: The published-content read side of the Payload REST + GraphQL API answers anonymously (GET /api/posts, /api/news, /api/pages, /api/media, /api/categories, /api/forms, /api/search, /api/redirects, /api/insights all return 200 without a token). /api/users returns 403 "You are not allowed to perform this action", so the access-control layer is present and selective, not absent.
  type: none
slug: spotwise-inc-authentication
source_filename: spotwise-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://spotwise.ai/.well-known/oauth-authorization-server,\n  https://app.spotwise.ai/.well-known/oauth-authorization-server,\n  https://spotwise.ai/api/auth/jwks, and live 401/403 probes of the MCP, CMS and\n  attribution surfaces\nnote: >-\n  Derived entirely from documents Spotwise itself serves. There is no published\n  OpenAPI and no public developer docs page, so nothing here comes from a written\n  auth guide — every field below was read off a live RFC 8414 / RFC 9728 metadata\n  document or observed on a real HTTP response.\n\nschemes:\n- id: spotwise_oauth2\n  type: oauth2\n  applies_to:\n  - https://spotwise.ai/api/mcp\n  - https://spotwise.ai/api (Payload CMS admin/write surface)\n  issuer: https://spotwise.ai/api/auth\n  flows:\n    authorization_code:\n      authorization_url: https://spotwise.ai/api/auth/oauth2/authorize\n      token_url: https://spotwise.ai/api/auth/oauth2/token\n      refresh_url: https://spotwise.ai/api/auth/oauth2/token\n\
  \      pkce: required-capable — code_challenge_methods_supported [S256]\n      scopes:\n        openid: OpenID Connect identity\n        profile: basic profile claims\n        email: email address claim\n        offline_access: refresh-token issuance\n        \"mcp:content.read\": read the site's Payload CMS content collections over MCP\n        \"mcp:content.write\": write the site's Payload CMS content collections over MCP\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  bearer_methods_supported:\n  - header\n\n- id: spotwise_app_oauth2\n  type: oauth2\n  applies_to:\n  - https://app.spotwise.ai/api/mcp\n  - https://app.spotwise.ai (product application)\n  issuer: https://app.spotwise.ai/api/auth\n  flows:\n    authorization_code:\n      authorization_url: https://app.spotwise.ai/api/auth/oauth2/authorize\n      token_url: https://app.spotwise.ai/api/auth/oauth2/token\n\
  \      refresh_url: https://app.spotwise.ai/api/auth/oauth2/token\n      pkce: required-capable — code_challenge_methods_supported [S256]\n      scopes:\n        openid: OpenID Connect identity\n        profile: basic profile claims\n        email: email address claim\n        offline_access: refresh-token issuance\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  bearer_methods_supported:\n  - header\n\n- id: spotwise_none\n  type: none\n  applies_to:\n  - https://spotwise.ai/api (Payload CMS public READ surface)\n  note: >-\n    The published-content read side of the Payload REST + GraphQL API answers\n    anonymously (GET /api/posts, /api/news, /api/pages, /api/media, /api/categories,\n    /api/forms, /api/search, /api/redirects, /api/insights all return 200 without a\n    token). /api/users returns 403 \"You are not allowed to perform this action\", so\n    the\
  \ access-control layer is present and selective, not absent.\n\nendpoints:\n  authorize: https://spotwise.ai/api/auth/oauth2/authorize\n  token: https://spotwise.ai/api/auth/oauth2/token\n  jwks: https://spotwise.ai/api/auth/jwks\n  registration: https://spotwise.ai/api/auth/oauth2/register\n  introspection: https://spotwise.ai/api/auth/oauth2/introspect\n  revocation: https://spotwise.ai/api/auth/oauth2/revoke\n  userinfo: https://spotwise.ai/api/auth/oauth2/userinfo\n  end_session: https://spotwise.ai/api/auth/oauth2/end-session\n\ntokens:\n  id_token_signing_alg_values_supported:\n  - EdDSA\n  jwks_key:\n    kty: OKP\n    crv: Ed25519\n    alg: EdDSA\n  claims_supported:\n  - sub\n  - iss\n  - aud\n  - exp\n  - iat\n  - sid\n  - scope\n  - azp\n  - email\n  - email_verified\n  - name\n  - picture\n  - family_name\n  - given_name\n  subject_types_supported:\n  - public\n\ncapabilities:\n  dynamic_client_registration: true\n  dynamic_client_registration_auth: none (public registration\
  \ permitted)\n  pkce: S256\n  introspection: true\n  revocation: true\n  rp_initiated_logout: true\n  authorization_response_iss_parameter_supported: true\n  response_types_supported:\n  - code\n  response_modes_supported:\n  - query\n  prompt_values_supported:\n  - login\n  - consent\n  - create\n  - select_account\n  - none\n  acr_values_supported:\n  - urn:mace:incommon:iap:bronze\n\napi_keys:\n  published: false\n  note: no API-key programme, key prefix, or credential-issuance page is published\n    anywhere on the public surface\n\noidc:\n  discovery_document_published: false\n  note: >-\n    /.well-known/openid-configuration returns 404 on every host, but the RFC 8414\n    authorization-server document carries OIDC fields (userinfo_endpoint,\n    id_token_signing_alg_values_supported, claims_supported, end_session_endpoint),\n    so the deployment is OIDC-capable while only advertising the OAuth metadata path.\n\nevidence:\n- url: https://spotwise.ai/.well-known/oauth-authorization-server\n\
  \  status: 200\n- url: https://app.spotwise.ai/.well-known/oauth-authorization-server\n  status: 200\n- url: https://spotwise.ai/api/auth/jwks\n  status: 200\n- url: https://spotwise.ai/api/mcp\n  status: 401\n- url: https://spotwise.ai/api/users\n  status: 403\n- url: https://spotwise.ai/.well-known/openid-configuration\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotwise-inc/refs/heads/main/authentication/spotwise-inc-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Broadcast Media
- Advertising
- Media Monitoring
- Sales Intelligence
- Lead Generation
- Artificial Intelligence
- Radio
- MCP
- Agents
- Attribution
---
