---
api_key_in: []
api_specs:
- filename: infoworks-rest-api-v3-openapi.yml
  format: yaml
  label: Infoworks REST API v3
  slug: infoworks-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoworks/refs/heads/main/openapi/infoworks-rest-api-v3-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Infoworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infoworks secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Infoworks
provider_slug: infoworks
scheme_count: 2
schemes:
- applied_to: 'Every non-/security operation in the spec declares security [{BearerAuth: []}] at the operation level. There is no root-level security block.'
  bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/infoworks-rest-api-v3-openapi.yml
  - https://docs.infoworks.io/developer-resources/rest-api
  token_lifetime: 15 minutes by default, configurable by the deployment administrator.
  type: http
- applied_to: GET /security/authenticate only (token minting).
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/infoworks-rest-api-v3-openapi.yml
  - https://docs.infoworks.io/developer-resources/rest-api
  type: http
slug: infoworks-authentication
source_filename: infoworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://docs.infoworks.io/developer-resources/rest-api\nderived_from: openapi/infoworks-rest-api-v3-openapi.yml\ndocs: https://docs.infoworks.io/developer-resources/rest-api\nsummary:\n  types: [http]\n  model: >-\n    Two-step: exchange a long-lived credential (HTTP Basic username:password, OR a refresh token\n    copied from the Infoworks UI) for a short-lived JWT bearer token, then send that JWT on every\n    subsequent call. There is no OAuth 2.0 authorization server and no API-key header, so there is no\n    scope surface to document — see scopes/ (deliberately absent).\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied_to: >-\n    Every non-/security operation in the spec declares security [{BearerAuth: []}] at the operation\n    level. There is no root-level security block.\n  token_lifetime: 15 minutes by default, configurable by the deployment administrator.\n  sources: [openapi/infoworks-rest-api-v3-openapi.yml,\
  \ https://docs.infoworks.io/developer-resources/rest-api]\n- name: BasicAuth\n  type: http\n  scheme: basic\n  applied_to: 'GET /security/authenticate only (token minting).'\n  sources: [openapi/infoworks-rest-api-v3-openapi.yml, https://docs.infoworks.io/developer-resources/rest-api]\nflows:\n- name: username-and-password\n  steps:\n  - Base64-encode \"<username>:<password>\".\n  - 'GET /v3/security/authenticate with header Authorization: Basic <encoded>.'\n  - Read the JWT from result.authentication_token in the response body.\n  - 'Send it on every subsequent call as Authorization: Bearer <token>.'\n  constraint: Cannot be used when the deployment authenticates via SAML.\n  operation: GET /security/authenticate\n  docs: https://docs.infoworks.io/developer-resources/rest-api\n- name: refresh-token\n  steps:\n  - In the Infoworks UI go to My Profile > Settings and copy the value in the Refresh Token section.\n  - 'GET /v3/security/token/access with header Authorization: Basic <refresh_token>.'\n\
  \  - Read the JWT from result.authentication_token.\n  constraint: >-\n    Works for any authentication mechanism, including SAML. Since v6.2.0 the platform enforces\n    refresh-token expiry with administrator-configurable duration and automated expiry notifications.\n  operation: GET /security/token/access\n  docs: https://docs.infoworks.io/developer-resources/rest-api\ntoken_management:\n  validate: GET /security/token/validate\n  revoke_access_token: DELETE /security/token/access (operationId deleteAuthToken, \"Purge authentication token\")\n  rotate_refresh_token: DELETE /security/token/refresh (\"Regenerate Refresh Token and blacklist old token\")\nenterprise_identity:\n  saml:\n    supported: true\n    evidence: 'GET /security/sso/initialise (\"Get SAML Redirect URL\") in the Security tag.'\n  ldap:\n    supported: true\n    evidence: 'POST /security/get/user/data (\"LDAP Authorise User\") and POST /security/bulk-ldap-sync.'\n  service_authentication:\n    supported: true\n    evidence:\
  \ >-\n      A five-operation \"Service Authentication\" tag plus \"Secret Store\"/\"Secrets\" tags manage\n      machine credentials and external secret stores (KEYVAULT / ADMIN config types appear in job-hook\n      environment variable schemas).\nnotes:\n- >-\n  The auth model is per-deployment, not per-tenant on a vendor host: because Infoworks runs in the\n  customer's own cloud, the token is issued by the customer's own Infoworks instance.\n- >-\n  No OAuth 2.0, no OpenID Connect discovery, no API-key scheme and no mTLS scheme are declared in the\n  spec or documented. /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  were probed on every reachable host and returned nothing (see well-known/infoworks-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infoworks/refs/heads/main/authentication/infoworks-authentication.yml
summary_line: http · 2 schemes
tags:
- Data Engineering
- Data Integration
- Data Ingestion
- Data Pipelines
- Workflow Orchestration
- Data Warehouse Modernization
- Databricks
- Snowflake
- Big Data
- ETL
- Enterprise Data Operations
- Self-Hosted
---
