---
api_key_in: []
auth_types:
- none
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Insurance Council Australia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Insurance Council of Australia secures its APIs with none and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Insurance Council of Australia
provider_slug: insurance-council-australia
scheme_count: 3
schemes:
- applies_to:
  - https://insurancecouncil.com.au/wp-json/wp/v2
  - https://insurancecouncil.com.au/feed/
  evidence: 'GET /wp-json/ returned HTTP 200 with "authentication": [] — WordPress advertises

    no authentication scheme on this install. Confirmed anonymous 200 on

    /wp/v2/pages, /wp/v2/media, /wp/v2/categories, /wp/v2/tags, /wp/v2/types,

    /wp/v2/taxonomies, /wp/v2/statuses, /wp/v2/search, /wp/v2/comments.

    '
  name: anonymous
  type: none
- applies_to:
  - https://memberportal.insurancecouncil.com.au/
  authorization_endpoint: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/authorize
  claims_supported:
  - emails
  - given_name
  - family_name
  - oid
  - sub
  - idp
  - tfp
  - iss
  - iat
  - exp
  - aud
  - acr
  - nonce
  - auth_time
  client_credentials: false
  discovery_status: 200
  dynamic_client_registration: false
  end_session_endpoint: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://icab2cprod.b2clogin.com/tfp/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/v2.0/
  jwks_uri: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/discovery/v2.0/keys
  name: azure-ad-b2c-oidc
  note: 'A human sign-in flow for member insurers, not an API authorization server. No

    client-credentials grant is advertised, the scope catalogue is limited to

    openid, and no registration endpoint is published.

    '
  openIdConnectUrl: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/v2.0/.well-known/openid-configuration
  response_types_supported:
  - code
  - code id_token
  - code token
  - code id_token token
  - id_token
  - id_token token
  - token
  - token id_token
  scopes_supported:
  - openid
  subject_types_supported:
  - pairwise
  token_endpoint: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
- applies_to:
  - https://insurancecouncil.com.au/wp-json/
  evidence: 'Write and administrative routes reject anonymous callers: GET /wp/v2/users

    returned 401 rest_user_cannot_view, POST /wp-json/mcp/mcp-adapter-default-server

    (JSON-RPC tools/list) returned 401 rest_forbidden, and

    /wp-json/wp-abilities/v1/abilities returned 401 rest_forbidden. The install

    registers /wp/v2/users/<id>/application-passwords routes, and CORS advertises

    Authorization and X-WP-Nonce in access-control-allow-headers, but no credential

    is issued to third parties.

    '
  name: wordpress-privileged
  public: false
  type: cookie+nonce / application-password
slug: insurance-council-australia-authentication
source_filename: insurance-council-australia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: live probes 2026-07-25 + https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/v2.0/.well-known/openid-configuration\nnote: |\n  Derived by probe rather than from an OpenAPI document — the Insurance Council of\n  Australia publishes no machine-readable API specification. There are two distinct\n  authentication realms on the estate: an anonymous public read surface (the\n  incidental WordPress REST API and the RSS feed, which require no credential at\n  all) and a member-only human sign-in gate (Azure AD B2C OpenID Connect) fronting\n  the member portal. No machine-to-machine credential, API key, or client\n  registration path is offered to third parties.\nsummary:\n  types:\n  - none\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  public_read_requires_auth: false\n  self_serve_registration: false\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n\
  \  - https://insurancecouncil.com.au/wp-json/wp/v2\n  - https://insurancecouncil.com.au/feed/\n  evidence: |\n    GET /wp-json/ returned HTTP 200 with \"authentication\": [] — WordPress advertises\n    no authentication scheme on this install. Confirmed anonymous 200 on\n    /wp/v2/pages, /wp/v2/media, /wp/v2/categories, /wp/v2/tags, /wp/v2/types,\n    /wp/v2/taxonomies, /wp/v2/statuses, /wp/v2/search, /wp/v2/comments.\n- name: azure-ad-b2c-oidc\n  type: openIdConnect\n  applies_to:\n  - https://memberportal.insurancecouncil.com.au/\n  openIdConnectUrl: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/v2.0/.well-known/openid-configuration\n  discovery_status: 200\n  issuer: https://icab2cprod.b2clogin.com/tfp/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/v2.0/\n  authorization_endpoint: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/authorize\n  token_endpoint: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/token\n\
  \  end_session_endpoint: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/oauth2/v2.0/logout\n  jwks_uri: https://icab2cprod.b2clogin.com/04c7fa07-b168-495f-9dcc-bcfceb1a274e/b2c_1_signin/discovery/v2.0/keys\n  response_types_supported:\n  - code\n  - code id_token\n  - code token\n  - code id_token token\n  - id_token\n  - id_token token\n  - token\n  - token id_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - pairwise\n  scopes_supported:\n  - openid\n  claims_supported:\n  - emails\n  - given_name\n  - family_name\n  - oid\n  - sub\n  - idp\n  - tfp\n  - iss\n  - iat\n  - exp\n  - aud\n  - acr\n  - nonce\n  - auth_time\n  client_credentials: false\n  dynamic_client_registration: false\n  note: |\n    A human sign-in flow for member insurers, not an API authorization server. No\n    client-credentials grant is advertised,\
  \ the scope catalogue is limited to\n    openid, and no registration endpoint is published.\n- name: wordpress-privileged\n  type: cookie+nonce / application-password\n  applies_to:\n  - https://insurancecouncil.com.au/wp-json/\n  public: false\n  evidence: |\n    Write and administrative routes reject anonymous callers: GET /wp/v2/users\n    returned 401 rest_user_cannot_view, POST /wp-json/mcp/mcp-adapter-default-server\n    (JSON-RPC tools/list) returned 401 rest_forbidden, and\n    /wp-json/wp-abilities/v1/abilities returned 401 rest_forbidden. The install\n    registers /wp/v2/users/<id>/application-passwords routes, and CORS advertises\n    Authorization and X-WP-Nonce in access-control-allow-headers, but no credential\n    is issued to third parties.\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ncross_references:\n  scopes: scopes/insurance-council-australia-scopes.yml\n  conventions: conventions/insurance-council-australia-conventions.yml\n\
  \  well_known: well-known/insurance-council-australia-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insurance-council-australia/refs/heads/main/authentication/insurance-council-australia-authentication.yml
summary_line: none/openIdConnect · 3 schemes
tags:
- Insurance
- Australia
- General Insurance
- Industry Association
- Property and Casualty
- Claims
- Catastrophe
- Risk Data
- Code of Practice
---
