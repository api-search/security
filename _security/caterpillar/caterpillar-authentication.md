---
anonymous_access: false
api_key_in: []
api_specs:
- filename: iso-15143-3-aemp-20-api-postman-collection
  format: yaml
  label: ISO 15143-3 (AEMP 2.0) API
  slug: iso-15143-3-aemp-api
  spec_type: Postman
  url: https://digital.cat.com/knowledge-hub/document/iso-15143-3-aemp-20-api-postman-collection
- filename: visionlink-apis-postman-collection
  format: yaml
  label: VisionLink APIs
  slug: visionlink-apis
  spec_type: Postman
  url: https://digital.cat.com/knowledge-hub/document/visionlink-apis-postman-collection
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Caterpillar Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- implicit
- password
- deviceCode
- tokenExchange
- jwtBearer
- saml2Bearer
- ciba
overview: Caterpillar secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, implicit, password, deviceCode, tokenExchange, jwtBearer, saml2Bearer, and ciba flow(s).
provider_name: Caterpillar
provider_slug: caterpillar
scheme_count: 2
schemes:
- documented_flow_for_apis: clientCredentials
  flows:
  - flow: clientCredentials
    note: The flow the Cat Digital developer guides document for API consumers — a client id and client secret issued on subscription approval are exchanged for an access token that expires after 60 minutes.
    tokenUrl: https://fedlogin.cat.com/as/token.oauth2
  - authorizationUrl: https://fedlogin.cat.com/as/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://fedlogin.cat.com/as/token.oauth2
  - deviceAuthorizationUrl: https://fedlogin.cat.com/as/device_authz.oauth2
    flow: deviceCode
  - backchannelAuthenticationUrl: https://fedlogin.cat.com/as/bc-auth.ciba
    flow: ciba
  issuer: https://fedlogin.cat.com
  name: CatDigitalOAuth2
  source: https://fedlogin.cat.com/.well-known/openid-configuration
  type: oauth2
- name: CatDigitalOIDC
  openIdConnectUrl: https://fedlogin.cat.com/.well-known/openid-configuration
  source: https://fedlogin.cat.com/.well-known/openid-configuration
  type: openIdConnect
slug: caterpillar-authentication
source_filename: caterpillar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://fedlogin.cat.com/.well-known/openid-configuration\ndocs: https://digital.cat.com/knowledge-hub/articles/iso-15143-3-aemp-20-api-developer-guide\nnote: >-\n  Caterpillar publishes no public OpenAPI, so this profile is not derived from a\n  spec. It is read from the live OAuth 2.0 / OpenID Connect discovery documents\n  served by Caterpillar's own PingFederate authorization server at\n  fedlogin.cat.com (HTTP 200, fetched 2026-09-05), cross-checked against the Cat\n  Digital ISO 15143-3 developer guide, which names the same token endpoint.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode, implicit, password, deviceCode, tokenExchange, jwtBearer, saml2Bearer, ciba]\n  token_lifetime: 60 minutes\n  bearer_token_in: Authorization header\nschemes:\n  - name: CatDigitalOAuth2\n    type: oauth2\n    issuer: https://fedlogin.cat.com\n    source: https://fedlogin.cat.com/.well-known/openid-configuration\n\
  \    documented_flow_for_apis: clientCredentials\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://fedlogin.cat.com/as/token.oauth2\n        note: >-\n          The flow the Cat Digital developer guides document for API consumers —\n          a client id and client secret issued on subscription approval are\n          exchanged for an access token that expires after 60 minutes.\n      - flow: authorizationCode\n        authorizationUrl: https://fedlogin.cat.com/as/authorization.oauth2\n        tokenUrl: https://fedlogin.cat.com/as/token.oauth2\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://fedlogin.cat.com/as/device_authz.oauth2\n      - flow: ciba\n        backchannelAuthenticationUrl: https://fedlogin.cat.com/as/bc-auth.ciba\n  - name: CatDigitalOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://fedlogin.cat.com/.well-known/openid-configuration\n    source: https://fedlogin.cat.com/.well-known/openid-configuration\nendpoints:\n  issuer:\
  \ https://fedlogin.cat.com\n  authorization: https://fedlogin.cat.com/as/authorization.oauth2\n  token: https://fedlogin.cat.com/as/token.oauth2\n  revocation: https://fedlogin.cat.com/as/revoke_token.oauth2\n  introspection: https://fedlogin.cat.com/as/introspect.oauth2\n  userinfo: https://fedlogin.cat.com/idp/userinfo.openid\n  jwks: https://fedlogin.cat.com/pf/JWKS\n  registration: https://fedlogin.cat.com/as/clients.oauth2\n  pushed_authorization_request: https://fedlogin.cat.com/as/par.oauth2\n  device_authorization: https://fedlogin.cat.com/as/device_authz.oauth2\n  backchannel_authentication: https://fedlogin.cat.com/as/bc-auth.ciba\n  end_session: https://fedlogin.cat.com/idp/init_logout.openid\ncapabilities:\n  pkce: [plain, S256]\n  dynamic_client_registration: true\n  pushed_authorization_requests: supported\n  require_pushed_authorization_requests: false\n  dpop_signing_algs: [RS256, RS384, RS512, ES256, ES384, ES512, PS256, PS384, PS512]\n  token_endpoint_auth_methods: [client_secret_basic,\
  \ client_secret_post, client_secret_jwt, private_key_jwt, tls_client_auth, none]\n  mtls_client_auth: true\n  token_exchange: true\n  request_object_signing: true\n  request_uri_parameter_supported: false\n  authorization_response_iss_parameter_supported: false\n  backchannel_logout: true\n  frontchannel_logout: true\nclaims_supported:\n  - catafltnclass\n  - catafltncode\n  - catcupid\n  - catloginid\n  - displayName\n  - givenName\n  - mail\n  - sn\n  - sub\n  - telephonenumber\ngaps:\n  - >-\n    token_endpoint_auth_methods_supported advertises `none`, and\n    id_token_signing_alg_values_supported advertises `none` — both are\n    PingFederate defaults rather than anything Caterpillar documents, but they\n    are what the discovery document actually says.\n  - >-\n    code_challenge_methods_supported still advertises `plain` alongside `S256`.\n  - >-\n    No /.well-known/oauth-protected-resource (RFC 9728) is served on any host, so\n    an agent holding a token cannot discover the\
  \ resource server from metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caterpillar/refs/heads/main/authentication/caterpillar-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Construction
- Engines
- Fortune 500
- Heavy Equipment
- Locomotives
- Manufacturing
- Mining
- Telematics
- Fleet Management
- ISO 15143-3
- AEMP
---
