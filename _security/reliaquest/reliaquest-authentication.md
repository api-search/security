---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: 2sAYQZJYMC
  format: yaml
  label: GreyMatter API
  slug: greymatter-api
  spec_type: Postman
  url: https://apidocs.myreliaquest.com/api/collections/39440280/2sAYQZJYMC?segregateAuth=true&versionTag=latest
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Reliaquest Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReliaQuest secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ReliaQuest
provider_slug: reliaquest
scheme_count: 2
schemes:
- api: reliaquest:greymatter-api
  description: Every GraphQL request to https://greymatter.myreliaquest.com/graphql must carry a dedicated high-entropy API key in an X-API-KEY header. Keys are minted in GreyMatter > Settings > API Key Management ("New API Key"), shown once at creation, and carry an expiration date (default one year). Normal email/password login credentials cannot be used. All calls must be HTTPS; plain HTTP and unauthenticated requests fail. ReliaQuest stores a one-way hash of the key.
  in: header
  key_policy:
    default_expiry: 1 year
    expiry_notification: none
    one_key_per_user: true
    renewal: not supported — create a new key; creating a new key invalidates the old one
    shown_once: true
    storage: one-way hash server-side
  management_operations:
  - createApiKey
  - deleteApiKeyById
  - deleteApiKeys
  - apiKeys
  multi_entity_header:
    name: x-reliaquest-customer
    purpose: override the account's default entity to pull data across company entities
    value: the customer headerSlug (from the `customer`/`customers` queries)
  name: greymatterApiKey
  parameter_name: X-API-KEY
  sources:
  - apidocs.myreliaquest.com
  type: apiKey
- api: reliaquest:searchlight-portal-api
  description: The SearchLight Portal API authenticates with HTTP Basic credentials (a portal API key id and secret sent as username/password) on every request to https://portal-digitalshadows.com/api/, with the vendor media type application/vnd.polaris-v38+json as both Content-Type and Accept. An unauthenticated request returns 401 with {"code":"PS229","status":401,"message":"Failed to authenticate ... Please contact drpsupport@reliaquest.com"}. Keys are issued inside the portal; the reference documentation is customer-only.
  name: searchlightBasic
  probed:
    checked: '2026-09-18'
    status: 401
    url: https://portal-digitalshadows.com/api/
  scheme: basic
  sources:
  - github.com/digitalshadows/shadowline-api
  - live probe
  type: http
slug: reliaquest-authentication
source_filename: reliaquest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: >-\n  https://apidocs.myreliaquest.com/ (GreyMatter API Postman documentation, \"Authentication\" and\n  \"Managing API Keys\" sections + collection-level auth block, fetched 2026-09-18) and\n  https://github.com/digitalshadows/shadowline-api (ReliaQuest/Digital Shadows' own SearchLight client,\n  shadowline/sl_constants.py + sl_helpers.py) corroborated by a live 401 from\n  https://portal-digitalshadows.com/api/ on 2026-09-18.\ndocs: https://apidocs.myreliaquest.com/\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [basic]\n  oauth2_flows: []\nschemes:\n  - name: greymatterApiKey\n    api: reliaquest:greymatter-api\n    type: apiKey\n    in: header\n    parameter_name: X-API-KEY\n    description: >-\n      Every GraphQL request to https://greymatter.myreliaquest.com/graphql must carry a dedicated\n      high-entropy API key in an X-API-KEY header. Keys are minted in GreyMatter > Settings > API Key\n\
  \      Management (\"New API Key\"), shown once at creation, and carry an expiration date (default one\n      year). Normal email/password login credentials cannot be used. All calls must be HTTPS; plain\n      HTTP and unauthenticated requests fail. ReliaQuest stores a one-way hash of the key.\n    key_policy:\n      one_key_per_user: true\n      shown_once: true\n      default_expiry: 1 year\n      renewal: not supported — create a new key; creating a new key invalidates the old one\n      expiry_notification: none\n      storage: one-way hash server-side\n    multi_entity_header:\n      name: x-reliaquest-customer\n      value: the customer headerSlug (from the `customer`/`customers` queries)\n      purpose: override the account's default entity to pull data across company entities\n    management_operations: [createApiKey, deleteApiKeyById, deleteApiKeys, apiKeys]\n    sources: [apidocs.myreliaquest.com]\n  - name: searchlightBasic\n    api: reliaquest:searchlight-portal-api\n    type:\
  \ http\n    scheme: basic\n    description: >-\n      The SearchLight Portal API authenticates with HTTP Basic credentials (a portal API key id and\n      secret sent as username/password) on every request to https://portal-digitalshadows.com/api/,\n      with the vendor media type application/vnd.polaris-v38+json as both Content-Type and Accept.\n      An unauthenticated request returns 401 with {\"code\":\"PS229\",\"status\":401,\"message\":\"Failed to\n      authenticate ... Please contact drpsupport@reliaquest.com\"}. Keys are issued inside the portal;\n      the reference documentation is customer-only.\n    probed:\n      url: https://portal-digitalshadows.com/api/\n      status: 401\n      checked: '2026-09-18'\n    sources: [github.com/digitalshadows/shadowline-api, live probe]\nnotes: >-\n  No OAuth 2.0 / OIDC surface is documented for either API and no discovery document is served\n  (see well-known/reliaquest-well-known.yml). No scopes artifact is emitted: the GreyMatter API\
  \ key\n  inherits the creating user's role/permissions (accessGroup, role and permissions queries exist in\n  the API) rather than declaring OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliaquest/refs/heads/main/authentication/reliaquest-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cybersecurity
- Security Operations
- Threat Detection
- Incident Response
- Threat Intelligence
- Digital Risk Protection
- AI Agents
- GraphQL
---
