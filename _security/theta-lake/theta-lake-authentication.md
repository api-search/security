---
api_key_in: []
api_specs:
- filename: theta-lake-openapi-original.yml
  format: yaml
  label: Theta Lake API
  slug: theta-lake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theta-lake/refs/heads/main/openapi/theta-lake-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Theta Lake Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Theta Lake secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Theta Lake
provider_slug: theta-lake
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT bearer API token obtained from the /token endpoint
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/theta-lake-openapi-original.yml
  type: http
- description: OAuth2.0 client-credentials flow (client_id + client_secret -> JWT)
  flows:
  - flow: clientCredentials
    grant_type: client_credentials
    scopes: 70
    tokenUrl: https://developer.thetalake.ai/api/v1/token
    token_delivery: request-body (x-www-form-urlencoded; x-receive-token-in request-body)
  name: ClientCredentials
  sources:
  - openapi/theta-lake-openapi-original.yml
  type: oauth2
slug: theta-lake-authentication
source_filename: theta-lake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/theta-lake-openapi-original.yml\ndocs: https://developer.thetalake.ai/\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  model: >-\n    Create an API key (client_id + client_secret) in the Theta Lake developer portal, exchange it\n    at POST /token via the OAuth2 client-credentials grant (RFC 6749) for a short-lived JWT bearer\n    access token (expires_in 3600s), then send it as `Authorization: Bearer <jwt>` on every call.\n    Tokens are scoped to a workspace and a data center and carry a permissions[] set enforced\n    per-operation (see scopes/theta-lake-scopes.yml). GET /token/context returns a token's\n    workspace, data_center, type (jwt|oauth|third_party), and granted permissions.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer API token obtained from the /token endpoint\n  sources:\n  - openapi/theta-lake-openapi-original.yml\n\
  - name: ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developer.thetalake.ai/api/v1/token\n    token_delivery: request-body (x-www-form-urlencoded; x-receive-token-in request-body)\n    grant_type: client_credentials\n    scopes: 70\n  description: OAuth2.0 client-credentials flow (client_id + client_secret -> JWT)\n  sources:\n  - openapi/theta-lake-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theta-lake/refs/heads/main/authentication/theta-lake-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Communications Governance
- Compliance
- Archiving
- Security
- Supervision
- eDiscovery
- Legal Hold
- Records Management
- Unified Communications
- AI Governance
- Regulatory Compliance
---
