---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Veir Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: VEIR secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: VEIR
provider_slug: veir
scheme_count: 2
schemes:
- id_token_signing_alg_values_supported:
  - RS256
  issuer: https://veir.com
  name: OpenIDConnect
  openIdConnectUrl: https://veir.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/veir-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
- flows:
  - authorizationUrl: https://veir.com/oauth/authorize
    flow: authorizationCode
    scopes:
      openid: OpenID Connect subject identifier
      profile: Basic profile claims
      read: Read access
    tokenUrl: https://veir.com/oauth/token
  - flow: clientCredentials
    scopes:
      read: Read access
    tokenUrl: https://veir.com/oauth/token
  name: OAuth2
  sources:
  - well-known/veir-openid-configuration.json
  type: oauth2
slug: veir-authentication
source_filename: veir-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://veir.com/.well-known/openid-configuration\ndocs: null\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  status: advertised-but-unresolvable\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://veir.com/.well-known/openid-configuration\n  issuer: https://veir.com\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  response_types_supported: [code]\n  sources: [well-known/veir-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://veir.com/oauth/authorize\n    tokenUrl: https://veir.com/oauth/token\n    scopes:\n      openid: OpenID Connect subject identifier\n      profile: Basic profile claims\n      read: Read access\n  - flow: clientCredentials\n    tokenUrl: https://veir.com/oauth/token\n    scopes:\n \
  \     read: Read access\n  sources: [well-known/veir-openid-configuration.json]\nprotected_resource:\n  source: well-known/veir-oauth-protected-resource.json\n  resource: https://veir.com\n  authorization_servers: [https://veir.com]\n  scopes_supported: [openid, profile, read]\ncaveats:\n- >-\n  VEIR publishes a syntactically valid OIDC discovery document, but none of the endpoints it\n  advertises resolve. Probed 2026-08-05: /oauth/authorize returned 404, /oauth/token returned\n  404, and the advertised jwks_uri /.well-known/jwks.json returned 404. The metadata is\n  present; the authorization server behind it is not reachable anonymously.\n- >-\n  No developer registration, client-credential issuance, or token documentation was found\n  anywhere on veir.com. Nothing on the public site explains what these scopes grant access to.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://veir.com/.well-known/openid-configuration\n    status: 200\n  - url: https://veir.com/.well-known/oauth-protected-resource\n\
  \    status: 200\n  - url: https://veir.com/oauth/authorize\n    status: 404\n  - url: https://veir.com/oauth/token\n    status: 404\n  - url: https://veir.com/.well-known/jwks.json\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veir/refs/heads/main/authentication/veir-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Energy
- Electricity
- Data Centers
- Infrastructure
- Superconductors
- Content
---
