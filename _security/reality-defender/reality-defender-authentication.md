---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Reality Defender Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- clientCredentials
overview: Reality Defender secures its APIs with apiKey, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and clientCredentials flow(s).
provider_name: Reality Defender
provider_slug: reality-defender
scheme_count: 2
schemes:
- applies_to: Reality Defender detection REST API (api.prd.realitydefender.xyz)
  in: header
  key_source: Generated in the Reality Defender platform settings at https://app.realitydefender.ai
  name: ApiKeyAuth
  notes: 'Primary authentication for all detection endpoints and the SDKs. SDKs read the key from a REALITY_DEFENDER_API_KEY environment variable; the MCP server accepts it via env or a per-request X-Api-Key header.

    '
  parameter_name: X-API-KEY
  type: apiKey
- applies_to: End-user sign-in to the Reality Defender web platform (Auth0 tenant)
  flows_supported:
  - authorizationCode
  - deviceCode
  - clientCredentials
  - implicit
  issuer: https://auth.app.realitydefender.ai/
  name: PlatformOIDC
  notes: 'This OAuth2/OIDC surface authenticates humans into the console; it does not issue tokens for the detection API, which uses the X-API-KEY scheme above.

    '
  openIdConnectUrl: https://auth.app.realitydefender.ai/.well-known/openid-configuration
  pkce:
  - S256
  - plain
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  - phone
  - address
  type: openIdConnect
slug: reality-defender-authentication
source_filename: reality-defender-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.realitydefender.com/api-reference/quickstart\ndocs: https://docs.realitydefender.com/api-reference/quickstart\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  api_key_name: X-API-KEY\n  oauth2_flows: [authorizationCode, deviceCode, clientCredentials]\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: X-API-KEY\n    applies_to: Reality Defender detection REST API (api.prd.realitydefender.xyz)\n    key_source: Generated in the Reality Defender platform settings at https://app.realitydefender.ai\n    notes: >\n      Primary authentication for all detection endpoints and the SDKs.\n      SDKs read the key from a REALITY_DEFENDER_API_KEY environment variable;\n      the MCP server accepts it via env or a per-request X-Api-Key header.\n  - name: PlatformOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://auth.app.realitydefender.ai/.well-known/openid-configuration\n\
  \    issuer: https://auth.app.realitydefender.ai/\n    applies_to: End-user sign-in to the Reality Defender web platform (Auth0 tenant)\n    flows_supported: [authorizationCode, deviceCode, clientCredentials, implicit]\n    scopes_supported: [openid, profile, email, offline_access, phone, address]\n    pkce: [S256, plain]\n    notes: >\n      This OAuth2/OIDC surface authenticates humans into the console; it does not\n      issue tokens for the detection API, which uses the X-API-KEY scheme above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reality-defender/refs/heads/main/authentication/reality-defender-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Deepfake Detection
- Artificial Intelligence
- Media Authentication
- Content Moderation
- Security
- Fraud Prevention
- Synthetic Media
- Machine Learning
---
