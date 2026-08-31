---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Meow Wolf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meow Wolf declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Meow Wolf
provider_slug: meow-wolf
scheme_count: 0
schemes: []
slug: meow-wolf-authentication
source_filename: meow-wolf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://auth.meowwolf.com/.well-known/openid-configuration\nnote: >-\n  Meow Wolf publishes no API authentication documentation, because it publishes no API.\n  This profile is derived entirely from a live, anonymous OIDC discovery document served\n  by the company's own identity host, auth.meowwolf.com — an Auth0 custom-domain tenant\n  (CNAME meowwolf-cd-swbu1coxwcncnddi.edge.tenants.auth0.com). It was found by following\n  https://meowwolf.com/sign-in, which redirects to the ticketing app carrying\n  ?iss=https%3A%2F%2Fauth.meowwolf.com%2F. This is consumer sign-in for the ticketing\n  and customer-portal apps, NOT a developer authorization surface: no client credentials\n  are issued to third parties, no scopes beyond the standard OIDC profile/email set are\n  defined, and no API audience is documented. Recorded because it is real, callable and\n  standards-conformant, and because it is the only machine-readable contract\
  \ on the\n  entire Meow Wolf estate.\nissuer: https://auth.meowwolf.com/\nprovider: Auth0 (custom domain)\nsecurity_schemes:\n- key: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.meowwolf.com/.well-known/openid-configuration\n  description: >-\n    OpenID Connect Discovery 1.0 document, HTTP 200 anonymous. Also served byte-identical\n    at /.well-known/oauth-authorization-server (RFC 8414).\n- key: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.meowwolf.com/authorize\n      tokenUrl: https://auth.meowwolf.com/oauth/token\n      refreshUrl: https://auth.meowwolf.com/oauth/token\n    clientCredentials:\n      tokenUrl: https://auth.meowwolf.com/oauth/token\n    deviceCode:\n      deviceAuthorizationUrl: https://auth.meowwolf.com/oauth/device/code\n      tokenUrl: https://auth.meowwolf.com/oauth/token\n- key: wordpress_application_passwords\n  type: http\n  scheme: basic\n  description: >-\n    Unrelated to the above. The WooCommerce\
  \ shop at shop.meowwolf.com advertises\n    WordPress application-password authorization at\n    https://shop.meowwolf.com/wp-admin/authorize-application.php, and wc/v3 returns 401\n    woocommerce_rest_cannot_view anonymously. Platform default, not a Meow Wolf program.\nendpoints:\n  authorization: https://auth.meowwolf.com/authorize\n  token: https://auth.meowwolf.com/oauth/token\n  userinfo: https://auth.meowwolf.com/userinfo\n  jwks: https://auth.meowwolf.com/.well-known/jwks.json\n  revocation: https://auth.meowwolf.com/oauth/revoke\n  registration: https://auth.meowwolf.com/oidc/register\n  device_authorization: https://auth.meowwolf.com/oauth/device/code\n  backchannel_authentication: https://auth.meowwolf.com/bc-authorize\n  mfa_challenge: https://auth.meowwolf.com/mfa/challenge\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n\
  - urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\npkce:\n  supported: true\n  code_challenge_methods:\n  - S256\n  - plain\ndpop:\n  supported: true\n  signing_algs:\n  - ES256\nid_token_signing_alg_values_supported:\n- HS256\n- RS256\n- PS256\njwks:\n  url: https://auth.meowwolf.com/.well-known/jwks.json\n  key_count: 2\n  algs:\n  - RS256\nobservations:\n- >-\n  Dynamic client registration is enabled (/oidc/register present), which is unusual for\n  a pure consumer-login tenant and is the closest thing on the estate to a\n  self-service developer on-ramp — but it is undocumented and unadvertised.\n- >-\n  The implicit and password\
  \ (ROPC) grants are both still enabled, which OAuth 2.1 and\n  the Auth0 hardening guidance both deprecate.\n- >-\n  code_challenge_methods_supported includes \"plain\" alongside S256; S256 only is the\n  recommended posture.\n- >-\n  Back-channel logout is supported, and global token revocation per connection is\n  exposed — a comparatively modern Auth0 tenant configuration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meow-wolf/refs/heads/main/authentication/meow-wolf-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Art
- Entertainment
- Immersive Experiences
- Event
- Ticketing
- Museums
- Tourism
- Retail
- Mobile Apps
---
