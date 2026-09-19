---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Pearson Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pearson declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Pearson
provider_slug: pearson
scheme_count: 1
schemes:
- discovery_url: https://developer.pearson.com/.well-known/openid-configuration
  dpop:
    algs:
    - RS256
    - RS384
    - RS512
    - ES256
    - ES384
    - ES512
    - EdDSA
    supported: true
  dynamic_client_registration: true
  endpoints:
    authorization: https://developer.pearson.com/services/oauth2/authorize
    end_session: https://developer.pearson.com/services/auth/idp/oidc/logout
    introspection: https://developer.pearson.com/services/oauth2/introspect
    jwks_uri: https://developer.pearson.com/id/keys
    registration: https://developer.pearson.com/services/oauth2/register
    revocation: https://developer.pearson.com/services/oauth2/revoke
    token: https://developer.pearson.com/services/oauth2/token
    userinfo: https://developer.pearson.com/services/oauth2/userinfo
  grant_types:
  - authorization_code
  - refresh_token
  id: pearson_developer_portal_oidc
  id_token_signing_algs:
  - RS256
  issuer: https://developer.pearson.com
  jwks_status: 200
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  platform: Salesforce Experience Cloud identity provider running on Pearson's own host. The scopes_supported list is the stock Salesforce platform scope set (see scopes/pearson-scopes.yml) rather than a Pearson-authored API scope vocabulary.
  protocol: OpenID Connect 1.0
  response_types:
  - code
  - token
  - token id_token
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: pearson-authentication
source_filename: pearson-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://developer.pearson.com/.well-known/openid-configuration\nnote: >-\n  Derived from the live OpenID Connect discovery document Pearson serves at\n  developer.pearson.com, captured verbatim at\n  well-known/pearson-openid-configuration.json. This describes the identity provider\n  that gates the Pearson Developers Network portal — it is the login in front of the\n  documentation, not an authorization surface for a customer-callable Pearson API.\n  Pearson publishes no anonymous authentication reference for any API product: every\n  page under developer.pearson.com answers 401 and SAML-redirects to Pearson's\n  corporate Entra ID tenant, federated into a Salesforce Experience Cloud community.\n\nschemes:\n  - id: pearson_developer_portal_oidc\n    type: openIdConnect\n    protocol: OpenID Connect 1.0\n    issuer: https://developer.pearson.com\n    discovery_url: https://developer.pearson.com/.well-known/openid-configuration\n\
  \    endpoints:\n      authorization: https://developer.pearson.com/services/oauth2/authorize\n      token: https://developer.pearson.com/services/oauth2/token\n      userinfo: https://developer.pearson.com/services/oauth2/userinfo\n      revocation: https://developer.pearson.com/services/oauth2/revoke\n      introspection: https://developer.pearson.com/services/oauth2/introspect\n      registration: https://developer.pearson.com/services/oauth2/register\n      end_session: https://developer.pearson.com/services/auth/idp/oidc/logout\n      jwks_uri: https://developer.pearson.com/id/keys\n    jwks_status: 200\n    grant_types:\n      - authorization_code\n      - refresh_token\n    response_types:\n      - code\n      - token\n      - token id_token\n    token_endpoint_auth_methods:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n    pkce:\n      supported: true\n      code_challenge_methods:\n        - S256\n    dpop:\n      supported: true\n      algs:\
  \ [RS256, RS384, RS512, ES256, ES384, ES512, EdDSA]\n    id_token_signing_algs:\n      - RS256\n    dynamic_client_registration: true\n    subject_types: [public]\n    platform: >-\n      Salesforce Experience Cloud identity provider running on Pearson's own host. The\n      scopes_supported list is the stock Salesforce platform scope set (see\n      scopes/pearson-scopes.yml) rather than a Pearson-authored API scope vocabulary.\n\nhistorical:\n  - id: learningstudio_oauth\n    status: retired\n    note: >-\n      The retired Pearson LearningStudio APIs documented OAuth 1.0a (signed with an\n      Application ID, Token Key Moniker and Secret) and OAuth 2. That documentation now\n      sits behind the portal login; the platform itself was retired (see\n      lifecycle/pearson-lifecycle.yml) and api.pearson.com answers\n      \"service that has been moved\".\n    source: https://developer.pearson.com/learningstudio/authentication\n    probed_status: 401\n\ngaps:\n  - No anonymous, machine-readable\
  \ authentication reference for any live Pearson API.\n  - >-\n    No /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource\n    document on any Pearson host (all 401/404 — see well-known/pearson-well-known.yml).\n  - >-\n    The Pearson VUE gateway at ws.pearsonvue.com publishes no discovery document and no\n    anonymous auth description.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pearson/refs/heads/main/authentication/pearson-authentication.yml
summary_line: 1 scheme
tags:
- Education
- Learning
- Assessment
- Certification
- Publishing
- EdTech
- Qualifications
- Testing
- Learning Management
- Workforce Skills
---
