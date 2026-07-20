---
api_key_in: []
api_specs:
- filename: dispatch-rest-v3-openapi.yml
  format: yaml
  label: Dispatch REST API v3
  slug: rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-rest-v3-openapi.yml
- filename: dispatch-files-v1-openapi.yml
  format: yaml
  label: Dispatch Files API v1
  slug: files-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-files-v1-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Dispatch Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
- refreshToken
overview: Dispatch secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, password, and refreshToken flow(s).
provider_name: Dispatch
provider_slug: dispatch
scheme_count: 2
schemes:
- description: OAuth 2.0 bearer token supplied in the Authorization header. Tokens are temporary; integrations must handle 401 and re-authenticate.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dispatch-rest-v3-openapi.yml
  - openapi/dispatch-files-v1-openapi.yml
  type: http
- flows:
  - audience: job sources / networks
    description: Authenticate as a job source. client_id is the account public key and client_secret the secret key, both issued by Dispatch on signup.
    flow: clientCredentials
    parameters:
    - grant_type
    - client_id
    - client_secret
  - audience: individual service providers
    description: Authenticate a single service provider. Dispatch recommends creating a separate user account with the "dispatcher" role for the integration so integration actions are distinguishable from real user actions.
    flow: password
    parameters:
    - grant_type
    - username
    - password
    - client_id
    - client_secret
  - description: Exchange the refresh token issued alongside the access token for a new access token.
    flow: refreshToken
    parameters:
    - grant_type
    - refresh_token
  name: oauth2
  refresh_url: https://api.dispatch.me/v3/oauth/token
  sandbox_token_url: https://api-sandbox.dispatch.me/v3/oauth/token
  scope_count: 0
  sources:
  - openapi/dispatch-rest-v3-openapi.yml
  token_response:
    fields:
    - access_token
    - token_type
    - created_at
    - expires_in
    - refresh_token
    token_type: bearer
  token_url: https://api.dispatch.me/v3/oauth/token
  type: oauth2
slug: dispatch-authentication
source_filename: dispatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/DispatchMe/v3-api-docs/blob/master/source/index.html.md#authentication\ndocs: https://github.com/DispatchMe/v3-api-docs\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  oauth2_flows: [clientCredentials, password, refreshToken]\n  api_key_in: []\n  scopes_documented: false\n  notes: >-\n    Dispatch secures its API with OAuth 2.0 bearer tokens. Two credential models exist:\n    job sources (warranty companies, manufacturers, lead-gen platforms) authenticate with\n    the client_credentials grant using a public/secret key pair, which grants access to\n    objects assigned to all service providers in their network; an individual service\n    provider authenticates with the resource-owner password grant. Dispatch publishes no\n    OAuth scope vocabulary - authorization is governed by an account-level ACL negotiated\n    with an account manager, so scopes/ is intentionally absent for this provider.\n\
  schemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      OAuth 2.0 bearer token supplied in the Authorization header. Tokens are temporary;\n      integrations must handle 401 and re-authenticate.\n    sources: [openapi/dispatch-rest-v3-openapi.yml, openapi/dispatch-files-v1-openapi.yml]\n  - name: oauth2\n    type: oauth2\n    token_url: https://api.dispatch.me/v3/oauth/token\n    refresh_url: https://api.dispatch.me/v3/oauth/token\n    sandbox_token_url: https://api-sandbox.dispatch.me/v3/oauth/token\n    scope_count: 0\n    flows:\n      - flow: clientCredentials\n        audience: job sources / networks\n        parameters: [grant_type, client_id, client_secret]\n        description: >-\n          Authenticate as a job source. client_id is the account public key and\n          client_secret the secret key, both issued by Dispatch on signup.\n      - flow: password\n        audience: individual service providers\n        parameters: [grant_type,\
  \ username, password, client_id, client_secret]\n        description: >-\n          Authenticate a single service provider. Dispatch recommends creating a separate\n          user account with the \"dispatcher\" role for the integration so integration\n          actions are distinguishable from real user actions.\n      - flow: refreshToken\n        parameters: [grant_type, refresh_token]\n        description: Exchange the refresh token issued alongside the access token for a new access token.\n    token_response:\n      fields: [access_token, token_type, created_at, expires_in, refresh_token]\n      token_type: bearer\n    sources: [openapi/dispatch-rest-v3-openapi.yml]\naccess_control:\n  model: account-level ACL\n  description: >-\n    A job source has full access to the transactional data it sends to Dispatch (the job\n    and all child objects). Access to organizations, their customers and their dispatchers\n    and technicians depends on the relationship: a first-party network grants\
  \ broader\n    access than a third-party network where the organization already receives work from\n    other sources. A user authenticated as a single service provider has access to all\n    objects within their own organization.\n  roles: [dispatcher, technician]\ncredential_issuance:\n  self_service: false\n  description: Credentials are issued by a Dispatch account manager on signup; there is no self-service key portal.\nrelated:\n  - conventions/dispatch-conventions.yml\n  - errors/dispatch-problem-types.yml\n  - sandbox/dispatch-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/authentication/dispatch-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Field Service
- Service Orchestration
- Work Orders
- Scheduling
- Contractor Networks
- Home Services
- Warranty
- Customer Experience
- Logistics
- Company
---
