---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Hakimo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hakimo declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Hakimo
provider_slug: hakimo
scheme_count: 0
schemes: []
slug: hakimo-authentication
source_filename: hakimo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  https://portal.hakimo.ai/assets/env.js (public runtime config, HTTP 200),\n  https://hakimo.us.auth0.com/.well-known/openid-configuration (HTTP 200), and unauthenticated\n  GETs against https://portal.hakimo.ai/v2/orm/* (HTTP 401), all probed 2026-08-22.\nstatus: undocumented-by-provider\nscored: false\nnote: >-\n  IMPORTANT — this artifact is NOT a claim that Hakimo documents its authentication. It does\n  not. There is no developer portal, no API reference and no auth page anywhere on hakimo.ai.\n  Everything below was established by probing public, unauthenticated surfaces; no credentials\n  were used and no access control was defeated. For that reason NO `Authentication` pointer is\n  wired into apis.yml — emitting one would credit Hakimo with published auth documentation it\n  has not published. This file exists so the measurement is on the record, not to move a score.\nsurfaces:\n- name: Hakimo customer portal (tenant\
  \ application API)\n  host: portal.hakimo.ai\n  base: https://portal.hakimo.ai/v2/orm/\n  public: false\n  documented: false\n  observed_challenge:\n    request: unauthenticated GET, no Authorization header\n    status: 401\n    content_type: application/json\n    body: '{\"message\":\"Invalid token\",\"status\":401}'\n    www_authenticate: absent\n  note: >-\n    Same-origin backend of the Angular portal SPA. It is a first-party application API, not a\n    published integration API: no reference, no spec, no key issuance flow, no rate-limit or\n    error documentation. Individual operation paths are deliberately NOT enumerated here.\nidentity_provider:\n  vendor: Auth0\n  tenant: hakimo.us.auth0.com\n  issuer: https://hakimo.us.auth0.com/\n  discovery: https://hakimo.us.auth0.com/.well-known/openid-configuration\n  discovery_status: 200\n  oauth_metadata: https://hakimo.us.auth0.com/.well-known/oauth-authorization-server\n  oauth_metadata_status: 200\n  audience: https://hakimo.ai/orm\n\
  \  client_id_public: HDsOi2UZ7NXiERiG16p1hWeWc73yJlFf\n  client_type: public SPA (no client secret; PKCE)\n  authorization_endpoint: https://hakimo.us.auth0.com/authorize\n  token_endpoint: https://hakimo.us.auth0.com/oauth/token\n  revocation_endpoint: https://hakimo.us.auth0.com/oauth/revoke\n  jwks_uri: https://hakimo.us.auth0.com/.well-known/jwks.json\n  device_authorization_endpoint: https://hakimo.us.auth0.com/oauth/device/code\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  note: >-\n    A dedicated Auth0 tenant, i.e. OAuth 2.0 / OIDC bearer tokens carried as\n    `Authorization: Bearer <JWT>` against the audience https://hakimo.ai/orm.\
  \ The scope set\n    advertised at the discovery endpoint is Auth0's stock OIDC set (openid, profile, email,\n    offline_access, ...); NO Hakimo-specific API scopes are published anywhere, so no\n    scopes/ artifact is derivable and none was written.\n  sso: >-\n    The portal exposes an SSO configuration surface to tenants, so enterprise customers\n    almost certainly federate their own IdP. Hakimo publishes no documentation of that setup.\nabsent:\n- api-key-issuance-flow\n- published-scope-reference\n- published-token-lifetime\n- published-auth-documentation\n- machine-readable-security-schemes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hakimo/refs/heads/main/authentication/hakimo-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Physical Security
- Video Surveillance
- Access Control
- Artificial Intelligence
- Computer-Vision
- Security Operations
- Remote Guarding
- Alarm Monitoring
- Facility Management
---
