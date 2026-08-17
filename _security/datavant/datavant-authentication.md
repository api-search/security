---
api_key_in: []
api_specs:
- filename: datavant-rest-api-openapi.yml
  format: yaml
  label: Datavant REST API
  slug: datavant-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-rest-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Datavant Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Datavant secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Datavant
provider_slug: datavant
scheme_count: 2
schemes:
- applied: global
  flows:
  - flow: clientCredentials
    note: 'The specification declares an EMPTY scopes map and no operation narrows `security[]`, so every operation carries the same undifferentiated `oauth2: []` requirement. There is no per-operation authorization surface published.'
    refreshUrl: https://api.datavant.io/v2/oauth2/token
    scopes: 0
    tokenUrl: https://api.datavant.io/v2/oauth2/token
  name: oauth2
  sources:
  - openapi/datavant-rest-api-openapi.yml
  type: oauth2
- applied: portal
  issuer: https://datavant.auth0.com/
  name: openIdConnect
  note: Not declared in the REST API specification. Probed live and captured verbatim to well-known/datavant-openid-configuration.json; it backs the Datavant Portal and the identity layer around the API rather than the REST operations themselves.
  openIdConnectUrl: https://auth.datavant.com/.well-known/openid-configuration
  sources:
  - well-known/datavant-openid-configuration.json
  type: openIdConnect
slug: datavant-authentication
source_filename: datavant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/datavant-rest-api-openapi.yml\ndocs: https://developer.datavant.com/docs\nnote: >-\n  Derived from the OpenAPI securitySchemes, then upgraded from two live anonymous probes:\n  the OAuth 2.0 token operation documented in the specification itself (POST /oauth2/token,\n  \"Authenticate with Orders API using Client Credentials\"), and Datavant's Auth0 discovery\n  documents served at auth.datavant.com. The REST API and the Datavant Portal are two\n  different authentication surfaces backed by the same identity provider tenant\n  (https://datavant.auth0.com/): the REST API uses OAuth 2.0 client credentials against\n  https://api.datavant.io/v2/oauth2/token, while the Portal and the Datavant CLI use a\n  long-lived generated application credential issued from the Portal Download page.\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n  oauth2_flows:\n    - clientCredentials\n  api_key_in: []\n  bearer_token: true\n\
  \  identity_provider: Auth0 (tenant https://datavant.auth0.com/, custom domain auth.datavant.com)\nschemes:\n  - name: oauth2\n    type: oauth2\n    applied: global\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.datavant.io/v2/oauth2/token\n        refreshUrl: https://api.datavant.io/v2/oauth2/token\n        scopes: 0\n        note: >-\n          The specification declares an EMPTY scopes map and no operation narrows\n          `security[]`, so every operation carries the same undifferentiated\n          `oauth2: []` requirement. There is no per-operation authorization surface\n          published.\n    sources:\n      - openapi/datavant-rest-api-openapi.yml\n  - name: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://auth.datavant.com/.well-known/openid-configuration\n    issuer: https://datavant.auth0.com/\n    applied: portal\n    note: >-\n      Not declared in the REST API specification. Probed live and captured verbatim to\n      well-known/datavant-openid-configuration.json;\
  \ it backs the Datavant Portal and the\n      identity layer around the API rather than the REST operations themselves.\n    sources:\n      - well-known/datavant-openid-configuration.json\ntoken_request:\n  method: POST\n  url: https://api.datavant.io/v2/oauth2/token\n  content_type: application/json\n  body_fields:\n    - grant_type\n    - client_id\n    - client_secret\n  grant_type: client_credentials\n  response_fields:\n    - access_token\n    - token_type\n    - expires_in\n  token_type: bearer\n  expires_in_seconds: 7200\n  source: openapi/datavant-rest-api-openapi.yml#/paths/~1oauth2~1token\nauthorization_server_metadata:\n  discovery:\n    openid_configuration: https://auth.datavant.com/.well-known/openid-configuration\n    oauth_authorization_server: https://auth.datavant.com/.well-known/oauth-authorization-server\n    jwks_uri: https://datavant.auth0.com/.well-known/jwks.json\n  grant_types_supported:\n    - client_credentials\n    - authorization_code\n    - refresh_token\n\
  \    - password\n    - implicit\n    - 'urn:ietf:params:oauth:grant-type:device_code'\n    - 'urn:ietf:params:oauth:grant-type:token-exchange'\n    - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported:\n    - client_secret_basic\n    - client_secret_post\n    - private_key_jwt\n    - none\n  code_challenge_methods_supported:\n    - S256\n    - plain\n  id_token_signing_alg_values_supported_note: RS256 (Auth0 default; see the captured discovery document)\nother_credentials:\n  - surface: Datavant Portal / Datavant CLI\n    mechanism: generated application credential (credentials.txt), piped to the CLI on stdin or supplied via the DV_USER_CREDENTIALS environment variable\n    lifetime: 10 years\n    issued_from: Datavant Portal Download page (login-gated)\n    note: >-\n      This is a separate credential from the REST API OAuth client. It is generated once\n      and cannot be viewed again; account admins are emailed before expiry.\n    source: https://aws.amazon.com/marketplace/pp/prodview-eolcfagze2ihw\n\
  gaps:\n  - No scopes are published for the REST API, so an agent cannot request least privilege.\n  - No mTLS, no API-key scheme, and no DPoP / proof-of-possession is declared.\n  - No token-introspection or revocation endpoint is documented for the REST API token issuer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/authentication/datavant-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Healthcare
- United States
- Interoperability
- Health Data
- De-Identification
- Tokenization
- Real-World Data
- Record Retrieval
- Data Connectivity
- Life Sciences
- HIPAA
- Medical Records
- Release of Information
- Privacy
- OAuth 2.0
- Health Information Exchange
---
