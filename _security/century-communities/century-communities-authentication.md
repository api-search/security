---
anonymous_access: false
api_key_in: []
auth_types: []
description: Century Communities publishes no developer portal and no hand-written authentication guide. This profile is read entirely from the OpenID Connect discovery document the company's own host serves at /.well-known/openid-configuration (HTTP 200, application/json, probed 2026-09-14), plus the JWKS it points at. Every value below is copied from that document; nothing is inferred.
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Century Communities Authentication
name_suffix: Authentication
oauth_flows: []
overview: Century Communities declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Century Communities
provider_slug: century-communities
scheme_count: 1
schemes:
- claims:
  - aud
  - exp
  - iat
  - iss
  - sub
  - profile
  - email
  - role
  credential_issuance: Not public. There is no self-service sign-up, client registration endpoint, or developer portal; the discovery document advertises no registration_endpoint, so clients must be provisioned by Century Communities.
  endpoints:
    authorization: https://www.centurycommunities.com/api/episerver/connect/authorize
    end_session: https://www.centurycommunities.com/api/episerver/connect/logout
    jwks: https://www.centurycommunities.com/.well-known/jwks
    token: https://www.centurycommunities.com/api/episerver/connect/token
    userinfo: https://www.centurycommunities.com/api/episerver/connect/userinfo
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  id: openid-connect
  id_token_signing_alg:
  - RS256
  issuer: https://www.centurycommunities.com/
  name: OpenID Connect / OAuth 2.0 (Optimizely CMS)
  openIdConnectUrl: https://www.centurycommunities.com/.well-known/openid-configuration
  parameters:
    claims_parameter_supported: false
    request_parameter_supported: false
    request_uri_parameter_supported: false
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  response_modes:
  - form_post
  - fragment
  - query
  response_types:
  - code
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: century-communities-authentication
source_filename: century-communities-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://www.centurycommunities.com/.well-known/openid-configuration\nprovider: Century Communities\nproviderId: century-communities\ndescription: >-\n  Century Communities publishes no developer portal and no hand-written authentication\n  guide. This profile is read entirely from the OpenID Connect discovery document the\n  company's own host serves at /.well-known/openid-configuration (HTTP 200,\n  application/json, probed 2026-09-14), plus the JWKS it points at. Every value below is\n  copied from that document; nothing is inferred.\nownership_note: >-\n  The authorization server is the one built into Optimizely (Episerver) CMS, which Century\n  Communities runs its public site on. It is a first-party surface in the sense that\n  matters here: the issuer is https://www.centurycommunities.com/, and every endpoint the\n  document names lives under that host and is operated by Century Communities. The\n  software is the vendor's;\
  \ the deployment, the keys and the tokens are the company's.\nschemes:\n  - id: openid-connect\n    type: openIdConnect\n    name: OpenID Connect / OAuth 2.0 (Optimizely CMS)\n    openIdConnectUrl: https://www.centurycommunities.com/.well-known/openid-configuration\n    issuer: https://www.centurycommunities.com/\n    endpoints:\n      authorization: https://www.centurycommunities.com/api/episerver/connect/authorize\n      token: https://www.centurycommunities.com/api/episerver/connect/token\n      userinfo: https://www.centurycommunities.com/api/episerver/connect/userinfo\n      end_session: https://www.centurycommunities.com/api/episerver/connect/logout\n      jwks: https://www.centurycommunities.com/.well-known/jwks\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n    response_types:\n      - code\n    response_modes:\n      - form_post\n      - fragment\n      - query\n    pkce:\n      supported: true\n      code_challenge_methods:\n\
  \        - S256\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n    id_token_signing_alg:\n      - RS256\n    claims:\n      - aud\n      - exp\n      - iat\n      - iss\n      - sub\n      - profile\n      - email\n      - role\n    subject_types:\n      - public\n    parameters:\n      claims_parameter_supported: false\n      request_parameter_supported: false\n      request_uri_parameter_supported: false\n    credential_issuance: >-\n      Not public. There is no self-service sign-up, client registration endpoint, or\n      developer portal; the discovery document advertises no registration_endpoint, so\n      clients must be provisioned by Century Communities.\nanonymous_surface:\n  note: >-\n    The Optimizely Content Delivery API on the same host answers unauthenticated. Probed\n    2026-09-14: GET /api/episerver/v3.0/site returned HTTP 200 with the live site\n    definition, and GET /api/episerver/v3.0/content/5 returned HTTP 200 with\
  \ the home-page\n    content tree. No key, no token, no Authorization header.\n  endpoints_probed:\n    - url: https://www.centurycommunities.com/api/episerver/v3.0/site\n      status: 200\n    - url: https://www.centurycommunities.com/api/episerver/v3.0/content/5\n      status: 200\ngaps:\n  - No first-party authentication documentation of any kind.\n  - No dynamic client registration endpoint advertised.\n  - No /.well-known/oauth-protected-resource document (404 on every host probed).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/century-communities/refs/heads/main/authentication/century-communities-authentication.yml
summary_line: 1 scheme
tags:
- Real Estate
- Homebuilding
- Construction
- Content Management
- Consumer
- Mortgage
---
