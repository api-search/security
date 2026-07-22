---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Oasis Labs Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Oasis Labs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Oasis Labs
provider_slug: oasis-labs
scheme_count: 1
schemes:
- audience: https://api.oasislabs.com/parcel
  client_authentication:
    client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer
    description: The client authenticates with a signed JWT client assertion (private_key_jwt) rather than a shared client secret. The SDK mints a short-lived JWT (default 1 hour lifetime) signed with the app's private key.
    method: private_key_jwt
  default_scopes:
  - parcel.full
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  token_url: https://auth.oasislabs.com/oauth/token
  type: oauth2
slug: oasis-labs-authentication
source_filename: oasis-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  github.com/oasislabs/parcel-clients typescript/src/token.ts + http.ts\n  (documented OAuth2 model of the official SDK)\ndocs: https://docs.oasislabs.com/parcel/latest\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  client_authentication: private_key_jwt\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://auth.oasislabs.com/oauth/token\n  grant_type: client_credentials\n  client_authentication:\n    method: private_key_jwt\n    client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n    description: >-\n      The client authenticates with a signed JWT client assertion (private_key_jwt)\n      rather than a shared client secret. The SDK mints a short-lived JWT\n      (default 1 hour lifetime) signed with the app's private key.\n  audience: https://api.oasislabs.com/parcel\n  default_scopes:\n  - parcel.full\nnotes:\
  \ >-\n  Access tokens are used as Bearer tokens against the Parcel API base\n  (https://api.oasislabs.com/parcel/v1) and storage endpoint\n  (https://storage.oasislabs.com/v1/parcel). Scope grammar is parcel.full or\n  parcel.<resource>.<action>; see scopes/oasis-labs-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oasis-labs/refs/heads/main/authentication/oasis-labs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Privacy
- Data Governance
- Confidential Computing
- Blockchain
- Differential Privacy
- Machine Learning
- Developer Platform
- Web3
---
