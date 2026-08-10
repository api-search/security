---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Finite State Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Finite State secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Finite State
provider_slug: finite-state
scheme_count: 4
schemes:
- applies_to: finite-state:platform-api
  challenge_body: 'API key required. Provide via X-Authorization header or Authorization: Bearer <token>'
  description: User-scoped API token created in the platform settings UI. Tokens are named, tied to an individual user account, and displayed masked (first and last two characters only) after creation.
  in: header
  name: PlatformApiToken
  parameter_name: X-Authorization
  source: live 401 challenge from https://app.finitestate.io/api/public/v0/
  type: apiKey
- applies_to: finite-state:platform-api
  description: 'The same platform API token may be presented as an "Authorization: Bearer <token>" header instead of X-Authorization.'
  name: PlatformBearerToken
  scheme: bearer
  source: live 401 challenge from https://app.finitestate.io/api/public/v0/
  type: http
- additional_parameters:
  - description: Tenant/organization identifier supplied by Finite State API management
    format: uuid
    in: request
    name: ORGANIZATION_CONTEXT
    required: true
  applies_to: finite-state:graphql-api
  description: Client-credentials exchange using a CLIENT_ID and CLIENT_SECRET issued by Finite State. The resulting bearer token is sent on each GraphQL request together with an ORGANIZATION_CONTEXT UUID that scopes the request to a tenant. No public scope catalogue is published.
  flows:
  - audience: https://platform.finitestate.io/api/v1/graphql
    flow: clientCredentials
    scopes: {}
    tokenUrl: https://platform.finitestate.io/api/v1/auth/token
  name: GraphQLClientCredentials
  source: https://github.com/FiniteStateInc/finite-state-sdk-python (TOKEN_URL, AUDIENCE constants in finite_state_sdk/__init__.py)
  type: oauth2
- applies_to: finite-state:a2a-content-api
  description: The A2A content API at https://finitestate.io/api/a2a is anonymous and read-only. The agent card declares an empty securitySchemes object and an empty security array, and an unauthenticated POST succeeds.
  name: None
  type: none
  verified: '2026-08-04'
slug: finite-state-authentication
source_filename: finite-state-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: probed 401 responses from https://app.finitestate.io/api/public/v0/*;\n  https://docs.finitestate.io/docs/settings/api-tokens/;\n  https://docs.finitestate.io/docs/getting-started/credentials-setup/;\n  https://github.com/FiniteStateInc/finite-state-sdk-python\ndocs: https://docs.finitestate.io/docs/settings/api-tokens/\nnote: 'No OpenAPI could be retrieved anonymously — the spec at\n  https://app.finitestate.io/api/docs/openapi.json returns 401 — so this profile is\n  searched from documentation, the official Python SDK source, and the live 401\n  challenge, not derived from securitySchemes.'\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  anonymous_surfaces: [a2a-content-api]\nschemes:\n- name: PlatformApiToken\n  type: apiKey\n  in: header\n  parameter_name: X-Authorization\n  applies_to: finite-state:platform-api\n  source: live 401 challenge from https://app.finitestate.io/api/public/v0/\n\
  \  challenge_body: 'API key required. Provide via X-Authorization header or\n    Authorization: Bearer <token>'\n  description: User-scoped API token created in the platform settings UI. Tokens\n    are named, tied to an individual user account, and displayed masked (first and\n    last two characters only) after creation.\n- name: PlatformBearerToken\n  type: http\n  scheme: bearer\n  applies_to: finite-state:platform-api\n  source: live 401 challenge from https://app.finitestate.io/api/public/v0/\n  description: 'The same platform API token may be presented as an\n    \"Authorization: Bearer <token>\" header instead of X-Authorization.'\n- name: GraphQLClientCredentials\n  type: oauth2\n  applies_to: finite-state:graphql-api\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://platform.finitestate.io/api/v1/auth/token\n    audience: https://platform.finitestate.io/api/v1/graphql\n    scopes: {}\n  source: https://github.com/FiniteStateInc/finite-state-sdk-python (TOKEN_URL,\n\
  \    AUDIENCE constants in finite_state_sdk/__init__.py)\n  description: Client-credentials exchange using a CLIENT_ID and CLIENT_SECRET\n    issued by Finite State. The resulting bearer token is sent on each GraphQL\n    request together with an ORGANIZATION_CONTEXT UUID that scopes the request to\n    a tenant. No public scope catalogue is published.\n  additional_parameters:\n  - name: ORGANIZATION_CONTEXT\n    in: request\n    format: uuid\n    required: true\n    description: Tenant/organization identifier supplied by Finite State API\n      management\n- name: None\n  type: none\n  applies_to: finite-state:a2a-content-api\n  description: The A2A content API at https://finitestate.io/api/a2a is anonymous\n    and read-only. The agent card declares an empty securitySchemes object and an\n    empty security array, and an unauthenticated POST succeeds.\n  verified: '2026-08-04'\ncli_and_ci_credentials:\n  environment_variables: [FS_TOKEN, FINITE_STATE_AUTH_TOKEN, FS_ENDPOINT,\n    FINITE_STATE_DOMAIN]\n\
  \  credential_file: ~/.finitestate/credential\n  file_permissions: must not be readable by group or others\ntoken_hygiene:\n  rotation_policy_published: false\n  expiry_published: false\n  scopes_published: false\n  leak_response: 'Finite State may automatically disable any API key that has\n    leaked publicly.'\n  guidance: 'Do not share your API key with others or expose it in the browser or\n    other client-side code.'\ngaps:\n- No OpenID Connect discovery document at /.well-known/openid-configuration on any\n  host (404).\n- No OAuth authorization-server metadata at /.well-known/oauth-authorization-server\n  on any host (404).\n- No published scope or permission catalogue for either the REST or GraphQL API.\n- No documented token expiry or rotation policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finite-state/refs/heads/main/authentication/finite-state-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Product Security
- Software Supply Chain Security
- SBOM
- Firmware Analysis
- Vulnerability Management
- Binary Analysis
- Connected Devices
- Compliance
- Cybersecurity
- IoT
---
