---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agora-real-estate-agora-content-api-openapi.yml
  format: yaml
  label: Agora Real Estate Agora Content API
  slug: agora-real-estate-agora-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/openapi/agora-real-estate-agora-content-api-openapi.yml
- filename: agora-real-estate-wordpress-content-api-openapi.yml
  format: yaml
  label: Agora Real Estate WordPress Content API
  slug: agora-real-estate-wordpress-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/openapi/agora-real-estate-wordpress-content-api-openapi.yml
- filename: agora-real-estate-o-embed-api-openapi.yml
  format: yaml
  label: Agora Real Estate o Embed API
  slug: agora-real-estate-o-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/openapi/agora-real-estate-o-embed-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Agora Real Estate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agora Real Estate declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Agora Real Estate
provider_slug: agora-real-estate
scheme_count: 0
schemes: []
slug: agora-real-estate-authentication
source_filename: agora-real-estate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://auth.agorareal.com/.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server (both HTTP 200, 2026-09-12), plus live header and error\n  observation on https://websiteapi.agorareal.com/wp-json and the tenant client-platform hosts.\nsummary: >-\n  Agora runs three distinct authentication surfaces and documents none of them for developers. The\n  public website content API is anonymous for reads and uses stock WordPress credentials for writes.\n  The Cortex AI product authenticates through a full OAuth 2.0 / OpenID Connect authorization server\n  on Agora's own domain. The tenant client platform authenticates through AWS Cognito behind a\n  session the API gateway will not route without.\nsurfaces:\n- name: Agora Website Content API\n  api: agora-real-estate:agora-website-content-api\n  base_url: https://websiteapi.agorareal.com/wp-json\n  anonymous_read: true\n  note: >-\n    Every sampled GET\
  \ on agora/v1 and the public wp/v2 read routes returned 200 with real data and no\n    credential. Write and privileged routes return 401 — observed {\"code\":\"rest_not_logged_in\"} on\n    /wp/v2/users/me and {\"code\":\"rest_forbidden\"} on /wp/v2/settings.\n  schemes:\n  - type: apiKey\n    in: header\n    name: X-WP-Nonce\n    description: >-\n      WordPress cookie-authentication nonce. Not documented by Agora; advertised by the API itself in\n      the Access-Control-Allow-Headers response header (Authorization, X-WP-Nonce,\n      Content-Disposition, Content-MD5, Content-Type).\n    evidence: https://websiteapi.agorareal.com/wp-json/agora/v1/get-categories\n  - type: http\n    scheme: basic\n    description: >-\n      WordPress application passwords over HTTP Basic in the Authorization header — the route index\n      declares /wp/v2/users/{user_id}/application-passwords, so the feature is enabled on this\n      install. Applies to write routes only.\n    evidence: https://websiteapi.agorareal.com/wp-json\n\
  - name: Agora Authorization Server (Cortex)\n  api: agora-real-estate:agora-authorization-server\n  base_url: https://auth.agorareal.com\n  schemes:\n  - type: openIdConnect\n    openIdConnectUrl: https://auth.agorareal.com/.well-known/openid-configuration\n    issuer: https://auth.agorareal.com\n    description: >-\n      OpenID Connect discovery served anonymously. RS256 ID tokens, public subject type, userinfo at\n      /oauth2/userinfo, introspection at /oauth2/introspection, JWKS at /oauth2/jwks.\n    evidence: https://auth.agorareal.com/.well-known/openid-configuration\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://auth.agorareal.com/oauth2/authorize\n        tokenUrl: https://auth.agorareal.com/oauth2/token\n        refreshUrl: https://auth.agorareal.com/oauth2/token\n        scopes:\n          openid: OpenID Connect authentication\n          profile: Basic profile claims\n          email: Email address claim\n          offline_access:\
  \ Refresh-token issuance\n      clientCredentials:\n        tokenUrl: https://auth.agorareal.com/oauth2/token\n        scopes: {}\n      deviceCode:\n        deviceAuthorizationUrl: https://auth.agorareal.com/oauth2/device_authorization\n        tokenUrl: https://auth.agorareal.com/oauth2/token\n        scopes: {}\n    pkce:\n      required_by_metadata: false\n      code_challenge_methods_supported:\n      - S256\n    token_endpoint_auth_methods_supported:\n    - none\n    - client_secret_basic\n    - client_secret_post\n    description: >-\n      RFC 8414 authorization-server metadata served anonymously. The deviceCode flow is not an\n      OpenAPI-standard flow key and is recorded here as declared by the provider\n      (urn:ietf:params:oauth:grant-type:device_code). client_credentials appears in the OIDC\n      discovery document's grant_types_supported but not in the RFC 8414 document — recorded as the\n      provider publishes it, not reconciled.\n    evidence: https://auth.agorareal.com/.well-known/oauth-authorization-server\n\
  \  deployment_note: >-\n    The authorization server is a WorkOS AuthKit instance served on Agora's own domain — the Cortex\n    sign-in host cortex.agorareal.com 303s to https://auth.agorareal.com/?client_id=client_01K8C8...\n    with a redirect_uri back to /auth/callback. Public client registration is not offered.\n- name: Agora Client Platform API\n  api: agora-real-estate:agora-client-platform-api\n  base_url: https://{tenant}.acp.agorareal.com/api\n  schemes: []\n  note: >-\n    No scheme can be established from the outside. Every anonymous request to /api and /api/* on the\n    demo tenant and on sampled live tenants returned nginx 502 with no WWW-Authenticate challenge.\n    The client-platform bundle calls /api/admin/cognito/* routes, so AWS Cognito is the identity\n    provider, but Agora publishes no authentication documentation for this API.\ngaps:\n- No developer-facing authentication documentation exists on agorareal.com.\n- No API-key issuance, client registration or token\
  \ guide is published for any surface.\n- >-\n    No /.well-known/oauth-protected-resource is served on any host, so no resource server advertises\n    which authorization server protects it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/authentication/agora-real-estate-authentication.yml
summary_line: 0 schemes
tags:
- Real-Estate
- Investment Management
- Private Equity
- Fund Administration
- Investor Relations
- Capital Raising
- Syndication
- Fund Accounting
- Investor Portal
- CRM
- Payments
- Content Management
- Software-as-a-Service
---
