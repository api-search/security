---
api_key_in:
- header
api_specs:
- filename: captivateiq-attribute-worksheets-api-openapi.yml
  format: yaml
  label: CaptivateIQ Attribute Worksheets API
  slug: captivateiq-attribute-worksheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-attribute-worksheets-api-openapi.yml
- filename: captivateiq-audit-logs-api-openapi.yml
  format: yaml
  label: CaptivateIQ Audit Logs API
  slug: captivateiq-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-audit-logs-api-openapi.yml
- filename: captivateiq-commission-plans-api-openapi.yml
  format: yaml
  label: CaptivateIQ Commission Plans API
  slug: captivateiq-commission-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-commission-plans-api-openapi.yml
- filename: captivateiq-dashboards-api-openapi.yml
  format: yaml
  label: CaptivateIQ Dashboards API
  slug: captivateiq-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-dashboards-api-openapi.yml
- filename: captivateiq-data-workbooks-api-openapi.yml
  format: yaml
  label: CaptivateIQ Data Workbooks API
  slug: captivateiq-data-workbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-data-workbooks-api-openapi.yml
- filename: captivateiq-data-worksheets-api-openapi.yml
  format: yaml
  label: CaptivateIQ Data Worksheets API
  slug: captivateiq-data-worksheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-data-worksheets-api-openapi.yml
- filename: captivateiq-employee-assumptions-api-openapi.yml
  format: yaml
  label: CaptivateIQ Employee Assumptions API
  slug: captivateiq-employee-assumptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-employee-assumptions-api-openapi.yml
- filename: captivateiq-employees-api-openapi.yml
  format: yaml
  label: CaptivateIQ Employees API
  slug: captivateiq-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-employees-api-openapi.yml
- filename: captivateiq-hierarchies-api-openapi.yml
  format: yaml
  label: CaptivateIQ Hierarchies API
  slug: captivateiq-hierarchies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-hierarchies-api-openapi.yml
- filename: captivateiq-jobs-api-openapi.yml
  format: yaml
  label: CaptivateIQ Jobs API
  slug: captivateiq-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-jobs-api-openapi.yml
- filename: captivateiq-metadata-api-openapi.yml
  format: yaml
  label: CaptivateIQ Metadata API
  slug: captivateiq-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-metadata-api-openapi.yml
- filename: captivateiq-payouts-api-openapi.yml
  format: yaml
  label: CaptivateIQ Payouts API
  slug: captivateiq-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-payouts-api-openapi.yml
- filename: captivateiq-report-models-api-openapi.yml
  format: yaml
  label: CaptivateIQ Report Models API
  slug: captivateiq-report-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-report-models-api-openapi.yml
- filename: captivateiq-transformation-worksheets-api-openapi.yml
  format: yaml
  label: CaptivateIQ Transformation Worksheets API
  slug: captivateiq-transformation-worksheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-transformation-worksheets-api-openapi.yml
- filename: captivateiq-uploads-api-openapi.yml
  format: yaml
  label: CaptivateIQ Uploads API
  slug: captivateiq-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-uploads-api-openapi.yml
- filename: captivateiq-users-api-openapi.yml
  format: yaml
  label: CaptivateIQ Users API
  slug: captivateiq-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-users-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Captivateiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: CaptivateIQ secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CaptivateIQ
provider_slug: captivateiq
scheme_count: 2
schemes:
- description: Token-based authentication with required prefix "Token"
  docs_quote: '"set the `Authorization` header to `Token <your token value>`"'
  format: Token <your token value>
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/captivateiq-openapi-original.yml
  - https://developers.captivateiq.com/docs/getting-started-with-captivateiq
  type: apiKey
- authorization_endpoint: https://app.captivateiq.com/o/authorize/
  client_registration: 'client_id_metadata_document_supported: true'
  description: Real RFC 8414 authorization-server metadata served at HTTP 200 on the app host. This OAuth surface is NOT documented anywhere in the public developer reference, which describes only static token auth; it was found by probe. The single advertised scope is read, so the OAuth path is read-only as published.
  discovery: https://app.captivateiq.com/.well-known/oauth-authorization-server
  documented_by_provider: false
  flow: authorizationCode
  format: Bearer <access token>
  grant_types:
  - authorization_code
  - refresh_token
  in: header
  introspection_endpoint: https://app.captivateiq.com/o/introspect/
  issuer: https://app.captivateiq.com
  name: oauth2AuthorizationCode
  parameter: Authorization
  pkce: S256 (required method advertised)
  ref: scopes/captivateiq-scopes.yml
  revocation_endpoint: https://app.captivateiq.com/o/revoke_token/
  scopes:
  - read
  sources:
  - https://app.captivateiq.com/.well-known/oauth-authorization-server
  - well-known/captivateiq-oauth-authorization-server.json
  token_endpoint: https://app.captivateiq.com/o/token/
  type: oauth2
slug: captivateiq-authentication
source_filename: captivateiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.captivateiq.com/docs/getting-started-with-captivateiq, https://app.captivateiq.com/.well-known/oauth-authorization-server\n  (probed 2026-08-13), openapi/captivateiq-openapi-original.yml\ndocs: https://developers.captivateiq.com/docs/getting-started-with-captivateiq\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2: true\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Token <your token value>\n  description: Token-based authentication with required prefix \"Token\"\n  docs_quote: '\"set the `Authorization` header to `Token <your token value>`\"'\n  sources:\n  - openapi/captivateiq-openapi-original.yml\n  - https://developers.captivateiq.com/docs/getting-started-with-captivateiq\n- name: oauth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  in: header\n  parameter:\
  \ Authorization\n  format: Bearer <access token>\n  discovery: https://app.captivateiq.com/.well-known/oauth-authorization-server\n  issuer: https://app.captivateiq.com\n  authorization_endpoint: https://app.captivateiq.com/o/authorize/\n  token_endpoint: https://app.captivateiq.com/o/token/\n  revocation_endpoint: https://app.captivateiq.com/o/revoke_token/\n  introspection_endpoint: https://app.captivateiq.com/o/introspect/\n  pkce: S256 (required method advertised)\n  grant_types:\n  - authorization_code\n  - refresh_token\n  scopes:\n  - read\n  client_registration: 'client_id_metadata_document_supported: true'\n  documented_by_provider: false\n  description: Real RFC 8414 authorization-server metadata served at HTTP 200 on the app host. This OAuth\n    surface is NOT documented anywhere in the public developer reference, which describes only static\n    token auth; it was found by probe. The single advertised scope is read, so the OAuth path is read-only\n    as published.\n  sources:\n\
  \  - https://app.captivateiq.com/.well-known/oauth-authorization-server\n  - well-known/captivateiq-oauth-authorization-server.json\n  ref: scopes/captivateiq-scopes.yml\ntoken_management:\n  where: CaptivateIQ app > user profile settings > API Tokens tab\n  creation: Enter a label and click create.\n  visibility: '\"Save the token value somewhere safe. It will never be shown again.\" — shown once at creation.'\n  rotation_policy: null\n  expiry: null\n  scopes: null\n  note: 'No token scopes, permission levels, or expiry are documented for static API tokens; the token\n    inherits the permissions of the CaptivateIQ user that created it. Scopes exist only on the separate,\n    undocumented OAuth surface — see scopes/captivateiq-scopes.yml.'\ngaps:\n- OAuth 2.0 is served but entirely undocumented — the developer reference names only token auth.\n- Only a read scope is advertised; OAuth clients cannot perform ciq/v1 writes.\n- No token expiry or rotation policy published for static API\
  \ tokens.\n- No /.well-known/openid-configuration or jwks.json (404) — OAuth 2.0, not OpenID Connect.\n- api.captivateiq.com WAF answers 403 for every /.well-known/ path, so the API host publishes no discovery.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/authentication/captivateiq-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Cloud Saas
- Sales Commissions
- Incentive Compensation Management
- Sales Performance Management
- Revenue Operations
- Finance
- Payouts
- Commission Plans
- Sales Compensation
---
