---
api_key_in: []
api_specs:
- filename: lawvu-api-openapi-original.yml
  format: yaml
  label: LawVu API
  slug: lawvu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-api-openapi-original.yml
- filename: lawvu-account-openapi-original.json
  format: json
  label: LawVu Account
  slug: lawvu-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-account-openapi-original.json
- filename: lawvu-matters-openapi-original.json
  format: json
  label: LawVu Matters
  slug: lawvu-matters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-matters-openapi-original.json
- filename: lawvu-contracts-openapi-original.json
  format: json
  label: LawVu Contracts
  slug: lawvu-contracts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-contracts-openapi-original.json
- filename: lawvu-fields-openapi-original.json
  format: json
  label: LawVu Fields
  slug: lawvu-fields
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-fields-openapi-original.json
- filename: lawvu-files-openapi-original.json
  format: json
  label: LawVu Files
  slug: lawvu-files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-files-openapi-original.json
- filename: lawvu-invoices-openapi-original.json
  format: json
  label: LawVu Invoices
  slug: lawvu-invoices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/openapi/lawvu-invoices-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lawvu Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: LawVu secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: LawVu
provider_slug: lawvu
scheme_count: 1
schemes:
- authorization_url_template: https://{web_host}/#/authorize
  client_secret: optional
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  hosts:
    api_host:
      production: api.lawvu.com
      sandbox: api-sandbox.lawvu.com
    web_host:
      production: go.lawvu.com
      sandbox: demo.lawvu.com
  name: OAuth2 Authorization Code
  pkce: not documented
  request_encoding: application/x-www-form-urlencoded
  scopes_documented: false
  token_format: JWT (base64-encoded), carries sub / name / organisationId / exp / iat claims
  token_operation: openapi/lawvu-account-openapi-original.json#post-v1-auth-token
  token_presentation: 'Authorization: Bearer {access_token}'
  token_url_template: https://{api_host}/account-apis/v1/auth/token
  type: oauth2
slug: lawvu-authentication
source_filename: lawvu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api-docs.lawvu.com/docs/guides/authentication\ndocs: https://api-docs.lawvu.com/docs/guides/authentication\nclient_management_docs: https://api-docs.lawvu.com/docs/guides/integration-clients\nnote: >-\n  The published OpenAPI documents for the LawVu API declare no components.securitySchemes,\n  so this profile is searched from the authentication guide rather than derived from the specs.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  bearer_token: true\n  api_keys: false\nschemes:\n- name: OAuth2 Authorization Code\n  type: oauth2\n  flow: authorizationCode\n  authorization_url_template: https://{web_host}/#/authorize\n  token_url_template: https://{api_host}/account-apis/v1/auth/token\n  token_operation: openapi/lawvu-account-openapi-original.json#post-v1-auth-token\n  hosts:\n    web_host:\n      production: go.lawvu.com\n      sandbox: demo.lawvu.com\n    api_host:\n      production: api.lawvu.com\n\
  \      sandbox: api-sandbox.lawvu.com\n  grant_types:\n  - authorization_code\n  - refresh_token\n  client_secret: optional\n  pkce: not documented\n  scopes_documented: false\n  token_format: JWT (base64-encoded), carries sub / name / organisationId / exp / iat claims\n  token_presentation: 'Authorization: Bearer {access_token}'\n  request_encoding: application/x-www-form-urlencoded\nrefresh_tokens:\n  single_use: true\n  rotation: a new access_token + refresh_token pair is issued on every refresh; the\n    previous refresh token is invalidated\n  lifetimes:\n  - condition: client_secret supplied in token requests\n    lifetime: 30 days\n  - condition: no client_secret supplied (public clients / SPAs)\n    lifetime: 1 day\n  unattended_use: >-\n    after the first interactive authorization the refresh token can maintain server-to-server\n    access indefinitely; the first token pair must always be obtained interactively\nredirect_uris:\n  scheme: HTTPS absolute URLs only (or http://localhost)\n\
  \  relative_paths_allowed: false\n  exact_match_required: true\n  per_request_data: use the OAuth `state` parameter, not a varying redirect_uri\n  whitelisting:\n    sandbox: any redirect URI accepted, no pre-registration\n    production: must be whitelisted by LawVu when the client is registered\nsecurity_model:\n  delegated: true\n  description: >-\n    every call made with a token issued through the authorization code flow executes under\n    the security context of the user who granted consent; that user's roles, permissions and\n    data-access restrictions apply to every request\nclient_registration:\n  self_service: true\n  location: LawVu app > Integrations > Custom Integrations\n  required_permission: Manage Integrations\n  client_secret_shown_once: true\n  client_secret_expires: true\n  sandbox_clients_migratable_to_production: false\ndeprecated_mechanisms:\n- name: Ocp-Apim-Subscription-Key\n  status: removed\n  date: '2024-02-26'\n  note: subscription keys are no longer required;\
  \ the header is ignored if supplied\n  source: https://api-docs.lawvu.com/docs/changelog\nerrors_reference: errors/lawvu-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lawvu/refs/heads/main/authentication/lawvu-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Legal
- Legal Technology
- Legal Operations
- Contract Lifecycle Management
- Matter Management
- Document Management
- Spend Management
- SaaS
- Workflow
---
