---
api_key_in: []
auth_types:
- http
description: 'ReqKey has exactly one credential model: a per-project secret root key sent as an HTTP Bearer token. There is no OAuth, no OIDC, no mTLS, no per-user token and no scope system — the root key is all-or-nothing over every resource in its project. Captured from the published authentication guide and the per- endpoint auth badges in the API reference; ReqKey publishes no OpenAPI, so no securitySchemes could be derived mechanically.'
kind: authentication
layout: security
method: searched
name: Reqkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReqKey secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ReqKey
provider_slug: reqkey
scheme_count: 1
schemes:
- bearer_format: opaque
  header: Authorization
  issued_by: ReqKey dashboard (project Settings)
  name: projectRootKey
  prefix: reqkey_
  rotation:
    behavior: Regenerates the root key and migrates every child resource to the new key. Consumer-facing API keys keep working; only project auth changes.
    docs: https://www.reqkey.com/docs/api/projects
    endpoint: POST /project/rootkey-reroll
  scheme: bearer
  scope: Full read/write over every resource in the project — APIs, plans, consumers, keys, validation, credits, analytics and ingestion.
  sources:
  - https://www.reqkey.com/docs/authentication
  - https://www.reqkey.com/docs/api/projects
  type: http
  value_format: Bearer reqkey_<opaque>
slug: reqkey-authentication
source_filename: reqkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://www.reqkey.com/docs/authentication\ndocs: https://www.reqkey.com/docs/authentication\ndescription: >-\n  ReqKey has exactly one credential model: a per-project secret root key sent as\n  an HTTP Bearer token. There is no OAuth, no OIDC, no mTLS, no per-user token\n  and no scope system — the root key is all-or-nothing over every resource in\n  its project. Captured from the published authentication guide and the per-\n  endpoint auth badges in the API reference; ReqKey publishes no OpenAPI, so no\n  securitySchemes could be derived mechanically.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  scopes: none\n  mfa_on_api: false\nschemes:\n  - name: projectRootKey\n    type: http\n    scheme: bearer\n    bearer_format: opaque\n    header: Authorization\n    value_format: 'Bearer reqkey_<opaque>'\n    prefix: reqkey_\n    issued_by: ReqKey dashboard (project Settings)\n    scope:\
  \ >-\n      Full read/write over every resource in the project — APIs, plans,\n      consumers, keys, validation, credits, analytics and ingestion.\n    rotation:\n      endpoint: POST /project/rootkey-reroll\n      behavior: >-\n        Regenerates the root key and migrates every child resource to the new\n        key. Consumer-facing API keys keep working; only project auth changes.\n      docs: https://www.reqkey.com/docs/api/projects\n    sources:\n      - https://www.reqkey.com/docs/authentication\n      - https://www.reqkey.com/docs/api/projects\nunauthenticated_operations:\n  - {method: GET, path: /health, note: 'Only GET is allowed; other methods return 403.'}\nconsumer_credentials:\n  description: >-\n    Distinct from ReqKey's own auth: the keys ReqKey MINTS for its customers'\n    end-consumers. These are the subject of POST /key/validate, not a way to\n    authenticate to ReqKey.\n  format: '<prefix>_<opaque>'\n  default_prefix: the project name\n  custom_prefix: 'the `prefix`\
  \ field on POST /key/create'\n  default_transport: X-API-Key request header (SDK default; `header`, `query` or `cookie` configurable)\n  carries_credits: false\n  note: >-\n    Credits and rate limits live on the consumer that owns the key, never on the\n    key itself.\n  docs: https://www.reqkey.com/docs/api/keys\nfailure_modes:\n  - {status: 401, meaning: missing or invalid project root key}\n  - {status: 403, meaning: 'resource belongs to a different project, or key/consumer disabled'}\n  - {status: 410, meaning: the project is soft-deleted and its root key no longer authenticates}\ngaps:\n  - >-\n    No scoped or restricted keys: the root key can create and delete everything\n    in the project, so there is no least-privilege credential to hand an agent\n    or a CI job.\n  - No OAuth 2.0 / OIDC surface, and no /.well-known/openid-configuration (probed 404).\n  - No published key-rotation schedule or expiry on the root key; rotation is manual via /project/rootkey-reroll.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reqkey/refs/heads/main/authentication/reqkey-authentication.yml
summary_line: http · 1 scheme
tags:
- APIKeys
- Authentication
- Authorization
- rate-limiting
- usage-metering
- api-analytics
- api-management
- Developer Tools
- middleware
- observability
---
