---
api_key_in:
- header
- query
api_specs:
- filename: lytics-api-v2-openapi.json
  format: json
  label: Lytics API v2
  slug: lytics-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-api-v2-openapi.json
- filename: lytics-api-v1-openapi.json
  format: json
  label: V1 Lytics API
  slug: lytics-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-api-v1-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lytics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lytics
provider_slug: lytics
scheme_count: 2
schemes:
- bearer_prefix: false
  example: 'Authorization: <token>'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/lytics-api-v1-openapi.json
  - openapi/lytics-api-v2-openapi.json
  type: apiKey
- description: Query-string alternative documented in the V1 Lytics API description and accepted on the v1 /api and /collect surfaces. Not declared as a securityScheme in the v2 spec.
  in: query
  name: AccessTokenQuery
  parameter: access_token
  sources:
  - openapi/lytics-api-v1-openapi.json
  type: apiKey
slug: lytics-authentication
source_filename: lytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/lytics-api-v1-openapi.json, openapi/lytics-api-v2-openapi.json\ndocs: https://docs.lytics.com/docs/access-tokens\nnote: >-\n  Baseline derived mechanically from both published OpenAPI documents, then upgraded from\n  the provider's own token documentation and from the auth contract Lytics publishes in\n  its agent-skills repo (references/auth.md). Lytics is an API-key provider: there is no\n  OAuth, no OIDC and no scope surface on its own API, so scopes/ is deliberately absent.\n  Authorization is carried as the RAW header value with NO `Bearer` prefix — the single\n  most common integration mistake against this API.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  bearer_prefix: false\n  example: 'Authorization: <token>'\n  sources:\n  - openapi/lytics-api-v1-openapi.json\n  - openapi/lytics-api-v2-openapi.json\n\
  - name: AccessTokenQuery\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: >-\n    Query-string alternative documented in the V1 Lytics API description and accepted on\n    the v1 /api and /collect surfaces. Not declared as a securityScheme in the v2 spec.\n  sources:\n  - openapi/lytics-api-v1-openapi.json\ntoken_management:\n  ui_path: Account > Security > Access Tokens\n  docs: https://docs.lytics.com/docs/access-tokens\n  admin_only: true\n  shown_once: true\n  expiry_options: ['7 days', '30 days', '90 days', 'No expiration']\n  role_scoped: true\n  note: >-\n    Tokens are role-scoped at creation (\"Each token can be tailored to have the precise\n    access needed and no more\") and the secret is displayed exactly once. Roles can be\n    predefined or granular permissions; the changelog records a one-step conversion from\n    predefined roles to granular permissions.\ntoken_types:\n  - name: Access Token\n    note: Role-scoped token created in the UI. The current\
  \ mechanism.\n  - name: User Auth Token\n    note: >-\n      User-specific, normally for the web admin but usable on the API; attributes actions\n      to that user and expires. Documented in the V1 OpenAPI description.\n  - name: API User\n    note: >-\n      Less privileged role, does not expire, but less action history is retained.\n      Documented in the V1 OpenAPI description.\nenvironment_variables:\n  - {name: LYTICS_API_TOKEN, required: true, note: 'Used by the provider-published Agent Skills and lio-client.'}\n  - {name: LYTICS_API_URL, required: false, default: 'https://api.lytics.io'}\n  - {name: LIOKEY, required: true, note: 'Used by the Go CLI (github.com/lytics/lytics).'}\nnetwork_controls:\n  ip_allowlisting:\n    supported: true\n    setting: api_ip_whitelist\n    format: CIDR (v4 or v6)\n    note: >-\n      Restricts both API access and admin access to the account. Documented in the V1\n      OpenAPI description.\n  account_security_settings:\n    docs: https://docs.lytics.com/docs/security\n\
  \    options: [logon session days, logon session timeout minutes, enforce password complexity, enforce password history, SSO (Enterprise plan)]\nmulti_account:\n  parameter: account_id\n  note: >-\n    A token may reach multiple accounts; account_id (query) selects the target and is\n    present on 1,321 of the 1,467 published operations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/authentication/lytics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Customer Data Platform
- CDP
- Personalization
- Segmentation
- User Profiles
- Behavioral Analytics
- Content Affinity
- Real-Time Data
- Marketing Automation
- Audience Activation
---
