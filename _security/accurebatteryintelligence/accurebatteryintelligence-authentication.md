---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Accurebatteryintelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: ACCURE Battery Intelligence declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ACCURE Battery Intelligence
provider_slug: accurebatteryintelligence
scheme_count: 1
schemes:
- applies_to: https://gateway.accure-platform.com
  audience: https://gateway.accure-platform.com
  client:
    client_id: zZhKAGNSgN8KEJd3RwtXKj9lsBD1K1wX
    kind: public
    note: A public OAuth client id, recorded because it is compiled into a publicly served JavaScript bundle and is not a secret under the OAuth public-client model.
    type: SPA / browser (auth0-spa-js + @auth0/auth0-react)
  description: Auth0-issued JWT bearer tokens. The API gateway is registered in the tenant as an Auth0 API whose identifier (audience) is the gateway URL itself.
  id: auth0_oidc
  issuer: https://production-accure.eu.auth0.com/
  openIdConnectUrl: https://production-accure.eu.auth0.com/.well-known/openid-configuration
  type: openIdConnect
slug: accurebatteryintelligence-authentication
source_filename: accurebatteryintelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://production-accure.eu.auth0.com/.well-known/openid-configuration\nname: ACCURE Battery Intelligence authentication profile\nsummary: >-\n  ACCURE's platform API gateway is protected by OAuth 2.0 / OpenID Connect via a\n  dedicated Auth0 tenant. There is no public OpenAPI securitySchemes block to derive\n  from and no published authentication documentation, so this profile is built entirely\n  from two things that can be observed without credentials: the OpenID Provider metadata\n  the tenant serves anonymously, and the public client configuration compiled into the\n  platform single-page application bundle.\nprovenance:\n  discovery_document: well-known/accurebatteryintelligence-openid-configuration.json\n  spa_bundle: https://accure-platform.com/assets/index-BiGHoC2c.js\n  note: >-\n    The SPA bundle is a public static asset. It carries a build-time environment block\n    (VITE_AUTH0_DOMAIN, VITE_AUTH0_CLIENT_ID, VITE_AUTH0_AUDIENCE)\
  \ — values that are\n    public by design for a browser-based OAuth public client. No credential was used and\n    no secret is recorded here.\nschemes:\n- id: auth0_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://production-accure.eu.auth0.com/.well-known/openid-configuration\n  issuer: https://production-accure.eu.auth0.com/\n  audience: https://gateway.accure-platform.com\n  applies_to: https://gateway.accure-platform.com\n  description: >-\n    Auth0-issued JWT bearer tokens. The API gateway is registered in the tenant as an\n    Auth0 API whose identifier (audience) is the gateway URL itself.\n  client:\n    kind: public\n    type: SPA / browser (auth0-spa-js + @auth0/auth0-react)\n    client_id: zZhKAGNSgN8KEJd3RwtXKj9lsBD1K1wX\n    note: >-\n      A public OAuth client id, recorded because it is compiled into a publicly served\n      JavaScript bundle and is not a secret under the OAuth public-client model.\nendpoints:\n  authorization: https://production-accure.eu.auth0.com/authorize\n\
  \  token: https://production-accure.eu.auth0.com/oauth/token\n  userinfo: https://production-accure.eu.auth0.com/userinfo\n  jwks: https://production-accure.eu.auth0.com/.well-known/jwks.json\n  revocation: https://production-accure.eu.auth0.com/oauth/revoke\n  end_session: https://production-accure.eu.auth0.com/oidc/logout\n  device_authorization: https://production-accure.eu.auth0.com/oauth/device/code\n  registration: https://production-accure.eu.auth0.com/oidc/register\n  backchannel_authentication: https://production-accure.eu.auth0.com/bc-authorize\n  mfa_challenge: https://production-accure.eu.auth0.com/mfa/challenge\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n\
  - http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\nresponse_types_supported:\n- code\n- token\n- id_token\n- code token\n- code id_token\n- token id_token\n- code token id_token\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\npkce:\n  supported: true\n  code_challenge_methods:\n  - S256\n  - plain\nid_token_signing_alg_values_supported:\n- HS256\n- RS256\n- PS256\ndpop:\n  supported: true\n  note: >-\n    dpop_signing_alg_values_supported is present in the tenant discovery document. This\n    is Auth0 platform capability, not evidence that ACCURE's gateway requires DPoP.\nscopes_supported:\n- openid\n- profile\n- offline_access\n- name\n- given_name\n- family_name\n- nickname\n- email\n- email_verified\n- picture\n- created_at\n- identities\n- phone\n- address\nsso:\n  claimed: true\n  evidence: https://www.accure.net/battery-analytics/battery-intelligence\n  note: >-\n   \
  \ ACCURE's product page states the platform supports single sign-on. The tenant\n    discovery document does not enumerate enterprise connections, so the identity\n    providers offered to customers are not observable anonymously.\ngaps:\n- >-\n  No API-level scopes are published. The scopes_supported list above is the Auth0\n  tenant's standard OIDC scope set; the permissions defined on the gateway API\n  (audience https://gateway.accure-platform.com) are not discoverable without a token,\n  so no scopes/ artifact is written.\n- >-\n  No published authentication documentation, key-issuance flow, or token-lifetime policy\n  exists on any ACCURE public surface.\n- >-\n  Every gateway route returns HTTP 403 (edge) or a Fastify 404 envelope to an anonymous\n  request; no unauthenticated read surface was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accurebatteryintelligence/refs/heads/main/authentication/accurebatteryintelligence-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Energy
- Battery
- Energy Storage
- Analytics
- Artificial Intelligence
- Internet of Things
- Electric Vehicles
- Germany
---
