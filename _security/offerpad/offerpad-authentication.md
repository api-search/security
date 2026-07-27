---
api_key_in: []
api_specs:
- filename: offerpad-wordpress-wp-v2-openapi.yml
  format: yaml
  label: Offerpad WordPress REST API
  slug: offerpad-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offerpad/refs/heads/main/openapi/offerpad-wordpress-wp-v2-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Offerpad Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Offerpad secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Offerpad
provider_slug: offerpad
scheme_count: 3
schemes:
- anonymous_read: true
  authorization_endpoint: https://www.offerpad.com/wp-admin/authorize-application.php
  description: WordPress application passwords, advertised in the wp-json discovery document under authentication.application-passwords. Credentials are issued interactively at https://www.offerpad.com/wp-admin/authorize-application.php and sent as HTTP Basic. Required for every write route and for reads in the edit context; anonymous callers get the view context only. Issuance requires an Offerpad WordPress account — there is no self-serve signup, so this is effectively staff-only.
  evidence:
  - finding: authentication.application-passwords.endpoints.authorization present
    source: https://www.offerpad.com/wp-json/
    status: 200
  - finding: '{"code":"rest_forbidden","message":"Sorry, you are not allowed to do that.","data":{"status":401}}'
    source: https://www.offerpad.com/wp-json/wp/v2/settings
    status: 401
  name: applicationPasswords
  scheme: basic
  sources:
  - openapi/offerpad-wordpress-wp-v2-openapi.yml
  - openapi/offerpad-wp-json-discovery.json
  surface: Offerpad WordPress REST API
  type: http
- code_challenge_methods_supported:
  - S256
  description: The private customer backend at https://helix.offerpad.com serves an RFC 8414 authorization-server metadata document anonymously. It delegates to an Okta custom authorization server. Public clients (the Offerpad Connect SPA and the Offerpad mobile apps) use authorization code with S256 PKCE; there is no public client registration, so third parties cannot obtain a client_id.
  evidence:
  - source: https://helix.offerpad.com/.well-known/oauth-authorization-server
    status: 200
  flows:
  - authorizationUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/authorize
    flow: authorizationCode
    issuer: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357
    scopes:
      email: Email address and verification status for the signed-in customer.
      openid: Issue an OpenID Connect ID token for the signed-in Offerpad customer.
      profile: Basic profile claims for the signed-in customer.
    tokenUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: offerpadHelixOAuth
  sources:
  - well-known/offerpad-helix-oauth-authorization-server.json
  surface: Offerpad Helix customer backend (private)
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- description: 'Full OpenID Connect Discovery 1.0 metadata, served anonymously. Endpoints: authorize, token, userinfo, jwks, introspect, revoke, end_session, device authorize, and pushed authorization requests (PAR). ID tokens are RS256 signed; DPoP signing algorithms are advertised. 32 standard claims are supported. The Okta org-level issuer (https://offerpad.okta.com) is also discoverable and adds a groups scope.'
  dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/authorize
    device_authorization: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/device/authorize
    end_session: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/logout
    introspection: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/introspect
    jwks: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/keys
    pushed_authorization_request: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/par
    registration: https://offerpad.okta.com/oauth2/v1/clients
    revocation: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/revoke
    token: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/token
    userinfo: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/userinfo
  evidence:
  - source: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/.well-known/openid-configuration
    status: 200
  - source: https://offerpad.okta.com/.well-known/openid-configuration
    status: 200
  id_token_signing_alg_values_supported:
  - RS256
  name: offerpadOkta
  openIdConnectUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/.well-known/openid-configuration
  sources:
  - well-known/offerpad-okta-openid-configuration.json
  - well-known/offerpad-okta-org-openid-configuration.json
  surface: Offerpad customer identity (Okta)
  type: openIdConnect
slug: offerpad-authentication
source_filename: offerpad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  Live probes: https://www.offerpad.com/wp-json/ discovery document,\n  https://helix.offerpad.com/.well-known/oauth-authorization-server,\n  https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/.well-known/openid-configuration,\n  and openapi/offerpad-wordpress-wp-v2-openapi.yml\nsummary:\n  types:\n    - http\n    - oauth2\n    - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n  self_serve: false\n  note: >-\n    Offerpad publishes no developer authentication documentation, no API key programme and\n    no client registration path. Both auth surfaces below were discovered by probing, not\n    from developer docs. Neither grants access to any real estate, listing, valuation or\n    transaction capability on a self-serve basis.\nschemes:\n  - name: applicationPasswords\n    type: http\n    scheme: basic\n    surface: Offerpad WordPress REST API\n    sources:\n      - openapi/offerpad-wordpress-wp-v2-openapi.yml\n\
  \      - openapi/offerpad-wp-json-discovery.json\n    description: >-\n      WordPress application passwords, advertised in the wp-json discovery document under\n      authentication.application-passwords. Credentials are issued interactively at\n      https://www.offerpad.com/wp-admin/authorize-application.php and sent as HTTP Basic.\n      Required for every write route and for reads in the edit context; anonymous callers\n      get the view context only. Issuance requires an Offerpad WordPress account — there is\n      no self-serve signup, so this is effectively staff-only.\n    authorization_endpoint: https://www.offerpad.com/wp-admin/authorize-application.php\n    anonymous_read: true\n    evidence:\n      - {source: 'https://www.offerpad.com/wp-json/', status: 200, finding: 'authentication.application-passwords.endpoints.authorization present'}\n      - {source: 'https://www.offerpad.com/wp-json/wp/v2/settings', status: 401, finding: '{\"code\":\"rest_forbidden\",\"message\":\"\
  Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'}\n  - name: offerpadHelixOAuth\n    type: oauth2\n    surface: Offerpad Helix customer backend (private)\n    sources:\n      - well-known/offerpad-helix-oauth-authorization-server.json\n    description: >-\n      The private customer backend at https://helix.offerpad.com serves an RFC 8414\n      authorization-server metadata document anonymously. It delegates to an Okta custom\n      authorization server. Public clients (the Offerpad Connect SPA and the Offerpad mobile\n      apps) use authorization code with S256 PKCE; there is no public client registration,\n      so third parties cannot obtain a client_id.\n    flows:\n      - flow: authorizationCode\n        issuer: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357\n        authorizationUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/authorize\n        tokenUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/token\n        scopes:\n \
  \         openid: Issue an OpenID Connect ID token for the signed-in Offerpad customer.\n          profile: Basic profile claims for the signed-in customer.\n          email: Email address and verification status for the signed-in customer.\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n    code_challenge_methods_supported:\n      - S256\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - client_secret_basic\n    evidence:\n      - {source: 'https://helix.offerpad.com/.well-known/oauth-authorization-server', status: 200}\n  - name: offerpadOkta\n    type: openIdConnect\n    surface: Offerpad customer identity (Okta)\n    openIdConnectUrl: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/.well-known/openid-configuration\n    sources:\n      - well-known/offerpad-okta-openid-configuration.json\n      - well-known/offerpad-okta-org-openid-configuration.json\n    description: >-\n      Full OpenID Connect Discovery 1.0 metadata,\
  \ served anonymously. Endpoints: authorize,\n      token, userinfo, jwks, introspect, revoke, end_session, device authorize, and pushed\n      authorization requests (PAR). ID tokens are RS256 signed; DPoP signing algorithms are\n      advertised. 32 standard claims are supported. The Okta org-level issuer\n      (https://offerpad.okta.com) is also discoverable and adds a groups scope.\n    endpoints:\n      authorization: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/authorize\n      token: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/token\n      userinfo: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/userinfo\n      jwks: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/keys\n      introspection: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/introspect\n      revocation: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/revoke\n      end_session: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/logout\n      device_authorization:\
  \ https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/device/authorize\n      pushed_authorization_request: https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/v1/par\n      registration: https://offerpad.okta.com/oauth2/v1/clients\n    id_token_signing_alg_values_supported:\n      - RS256\n    dpop_signing_alg_values_supported:\n      - RS256\n      - RS384\n      - RS512\n      - ES256\n      - ES384\n      - ES512\n    evidence:\n      - {source: 'https://offerpad.okta.com/oauth2/ausftur6n2aTu6Sur357/.well-known/openid-configuration', status: 200}\n      - {source: 'https://offerpad.okta.com/.well-known/openid-configuration', status: 200}\nnot_found:\n  - api_keys: No API key programme, key management console or key documentation exists on any Offerpad host.\n  - mutual_tls: No mTLS surface advertised.\n  - partner_auth: >-\n      The Direct+, Powered By Offerpad, homebuilder and vendor partner programmes are gated\n      behind intake forms and an NDA; no programmatic credential\
  \ is described anywhere.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offerpad/refs/heads/main/authentication/offerpad-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Real Estate
- United States
- iBuyer
- PropTech
- Property Listings
- Brokerage
- MLS
- Cash Offer
- Renovation
- Home Buying
---
