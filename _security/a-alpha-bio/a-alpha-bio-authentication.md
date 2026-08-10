---
api_key_in: []
api_specs:
- filename: a-alpha-bio-datasets-api-openapi.yml
  format: yaml
  label: A-Alpha Bio Datasets API
  slug: a-alpha-bio-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a-alpha-bio/refs/heads/main/openapi/a-alpha-bio-datasets-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: A Alpha Bio Authentication
name_suffix: Authentication
oauth_flows: []
overview: A-Alpha Bio secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: A-Alpha Bio
provider_slug: a-alpha-bio
scheme_count: 2
schemes:
- bearer_format: JWT
  description: 'Declared on all nine operations of the Data Product API. Carries an AWS Cognito access token; the Atlas SPA attaches it via an axios request interceptor over the `Authorization: Bearer <token>` header.'
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/a-alpha-bio-atlas-data-product-openapi-original.json
  - openapi/a-alpha-bio-atlas-datasets-openapi.yml
  type: http
- description: Not declared in the OpenAPI. Observed in the Atlas web client's published JavaScript bundle, which configures AWS Amplify `Auth.Cognito` with `loginWith.oauth` (authorization-code response type, redirect to `<origin>/callback`) and the four scopes above. These are Cognito sign-in scopes, not per-resource API scopes — the Data Product API declares no scope requirements of its own, so no `scopes/` artifact is emitted.
  flow: authorizationCode
  name: CognitoHostedUI
  provider: AWS Cognito user pool (hosted UI)
  response_type: code
  scopes_requested:
  - openid
  - email
  - profile
  - aws.cognito.signin.user.admin
  sources:
  - https://atlas.aalphabio.com/assets/App-DfcS_Q-d.js
  type: oauth2
slug: a-alpha-bio-authentication
source_filename: a-alpha-bio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://api.atlas.aalphabio.com/openapi.json\ndocs: https://atlas.aalphabio.com/\nsummary:\n  types:\n  - http\n  - oauth2\n  style: >-\n    HTTP bearer JWT on the Atlas Data Product API. The token is minted by an AWS Cognito user pool through the hosted\n    OAuth 2.0 authorization-code flow that the Atlas web client runs; the API itself only ever sees the bearer header.\n  anonymous_access: partial\n  anonymous_note: >-\n    Verified live 2026-08-06: dataset discovery, dataset metadata and Data Cards answer with no Authorization header at\n    all; the data / schema / structures operations return 401 {\"detail\":\"Missing token\"}. An invalid bearer token is\n    NOT rejected on the anonymous-readable operations — GET /api/v1/datasets with `Authorization: Bearer invalid`\n    returns 200 with an empty `objects` array rather than a 401, so a bad token is treated as \"no entitlements\", not\n    as an authentication failure.\n\
  schemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Declared on all nine operations of the Data Product API. Carries an AWS Cognito access token; the Atlas SPA attaches\n    it via an axios request interceptor over the `Authorization: Bearer <token>` header.\n  sources:\n  - openapi/a-alpha-bio-atlas-data-product-openapi-original.json\n  - openapi/a-alpha-bio-atlas-datasets-openapi.yml\n- name: CognitoHostedUI\n  type: oauth2\n  flow: authorizationCode\n  response_type: code\n  provider: AWS Cognito user pool (hosted UI)\n  scopes_requested:\n  - openid\n  - email\n  - profile\n  - aws.cognito.signin.user.admin\n  description: >-\n    Not declared in the OpenAPI. Observed in the Atlas web client's published JavaScript bundle, which configures AWS\n    Amplify `Auth.Cognito` with `loginWith.oauth` (authorization-code response type, redirect to `<origin>/callback`)\n    and the four scopes above. These are Cognito sign-in scopes, not\
  \ per-resource API scopes — the Data Product API\n    declares no scope requirements of its own, so no `scopes/` artifact is emitted.\n  sources:\n  - https://atlas.aalphabio.com/assets/App-DfcS_Q-d.js\nclients:\n- name: Atlas web client\n  url: https://atlas.aalphabio.com/\n  flow: Cognito hosted-UI authorization code, token attached as bearer by the SPA\n- name: Atlas CLI client\n  url: https://atlas.aalphabio.com/cli-login\n  flow: >-\n    Browser-assisted device-style login — the `/cli-login` page signs the user in against the same Cognito domain and\n    then displays a short-lived \"login code\" the user pastes back into the terminal to finish signing in to the Atlas\n    client. See cli/a-alpha-bio-cli.yml.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://api.atlas.aalphabio.com/openapi.json\n    http_status: 200\n    note: OpenAPI 3.1.0, components.securitySchemes.HTTPBearer = {type http, scheme bearer}\n  - url: https://api.atlas.aalphabio.com/api/v1/datasets\n\
  \    http_status: 200\n    note: no Authorization header sent; returns {\"objects\":[]}\n  - url: https://api.atlas.aalphabio.com/api/v1/datasets?include_locked=true&include_coming_soon=true\n    http_status: 200\n    note: no Authorization header sent; returns 16 public dataset records\n  - url: https://api.atlas.aalphabio.com/api/v1/datasets/ab1001/data\n    http_status: 401\n    note: '{\"detail\":\"Missing token\"}'\n  - url: https://api.atlas.aalphabio.com/api/v1/datasets/ab1001/schema\n    http_status: 401\n    note: '{\"detail\":\"Missing token\"}'\n  - url: https://atlas.aalphabio.com/assets/App-DfcS_Q-d.js\n    http_status: 200\n    note: Amplify Cognito OAuth config with the four requested scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a-alpha-bio/refs/heads/main/authentication/a-alpha-bio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- protein-interactions
- biotechnology
- drug-discovery
- antibody-engineering
- synthetic-biology
- machine-learning
- training-data
- data-licensing
- life-sciences
- datasets
- protein-design
- bioinformatics
---
