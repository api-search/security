---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Unison Computing Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Unison Computing secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Unison Computing
provider_slug: unison-computing
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.unison-lang.org/oauth/authorize
    flow: authorizationCode
    pkce: required
    tokenUrl: https://api.unison-lang.org/oauth/token
  issuer: https://api.unison-lang.org
  jwks_uri: https://api.unison-lang.org/.well-known/jwks.json
  name: unison-share-oauth
  response_types_supported:
  - code
  sources:
  - well-known/unison-computing-openid-configuration.json
  - https://github.com/unisoncomputing/share-api
  type: oauth2
  userinfo_endpoint: https://api.unison-lang.org/user-info
slug: unison-computing-authentication
source_filename: unison-computing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.unison-lang.org/.well-known/openid-configuration\ndocs: https://github.com/unisoncomputing/share-api\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  token_signing: EdDSA (Ed25519)\nnotes: >\n  Unison Share (share-api, open source) acts as the authentication server for\n  UCM and Unison Cloud. It implements OAuth2 (RFC 6749) with the PKCE\n  extension and a subset of the OpenID Connect Core and OpenID Connect\n  Discovery specifications. Live OIDC discovery document is published at\n  https://api.unison-lang.org/.well-known/openid-configuration (saved in\n  well-known/), with an EdDSA/Ed25519 JWKS at /.well-known/jwks.json.\nschemes:\n  - name: unison-share-oauth\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.unison-lang.org/oauth/authorize\n        tokenUrl: https://api.unison-lang.org/oauth/token\n        pkce:\
  \ required\n    issuer: https://api.unison-lang.org\n    jwks_uri: https://api.unison-lang.org/.well-known/jwks.json\n    userinfo_endpoint: https://api.unison-lang.org/user-info\n    response_types_supported: [code]\n    sources:\n      - well-known/unison-computing-openid-configuration.json\n      - https://github.com/unisoncomputing/share-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unison-computing/refs/heads/main/authentication/unison-computing-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Programming Languages
- Cloud Computing
- Developer Tools
- Functional Programming
- Distributed Systems
- Platform as a Service
---
