---
api_key_in:
- header
- query
api_specs:
- filename: healthie-webhooks-asyncapi.yml
  format: yaml
  label: Healthie GraphQL API
  slug: healthie-graphql-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthie/refs/heads/main/asyncapi/healthie-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Healthie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Healthie secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Healthie
provider_slug: healthie
scheme_count: 4
schemes:
- description: The API key is sent in the Authorization header using the literal scheme word "Basic" followed by the raw key. Despite the scheme name this is NOT HTTP Basic authentication — the value is the API key itself, not a base64 user:password pair.
  format: Basic <API_KEY>
  in: header
  name: HealthieApiKey
  parameter_name: Authorization
  required: true
  source: https://docs.gethealthie.com/guides/api-concepts/authentication
  type: apiKey
- description: Constant discriminator header that must accompany every authenticated API request. Distinguishes API-key traffic from Healthie's own first-party session traffic.
  format: API
  in: header
  name: AuthorizationSource
  parameter_name: AuthorizationSource
  required: true
  source: https://docs.gethealthie.com/guides/api-concepts/authentication
  type: apiKey
- description: Required only for customers whose data is hosted in a dedicated Healthie shard. The shard ID is not self-service — Healthie issues it on request to hello@gethealthie.com.
  format: <SHARD_AUTHORIZATION_ID>
  in: header
  name: AuthorizationShard
  parameter_name: AuthorizationShard
  required: conditional
  source: https://docs.gethealthie.com/guides/api-concepts/authentication
  type: apiKey
- applies_to: GraphQL subscriptions over WebSocket
  description: 'The WebSocket protocol has no header phase, so Healthie carries the API key as a URL query parameter on the subscription connection. Note the security consequence: a long-lived PHI-bearing credential travels in a URL and is therefore exposed to proxy and connection logs in a way the header-based REST/GraphQL path is not.'
  format: wss://ws.gethealthie.com/subscriptions?token=<API_KEY>
  in: query
  name: WebsocketToken
  parameter_name: token
  required: true
  source: https://docs.gethealthie.com/guides/websockets-and-subscriptions/getting-started/
  type: apiKey
slug: healthie-authentication
source_filename: healthie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.gethealthie.com/guides/api-concepts/authentication\ndocs: https://docs.gethealthie.com/guides/api-concepts/authentication\nnote: >-\n  Healthie publishes no OpenAPI, so this profile could not be produced by\n  0-working/derive-authentication.py (which reads OpenAPI securitySchemes). It was read directly from\n  the published authentication guide and cross-checked against the GraphQL schema captured in\n  graphql/healthie-schema.graphql (the createApiKey mutation and ApiKey type exist verbatim).\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  mtls: false\n  model: static per-user API key; permissions are inherited from the Healthie user account the key\n    is attached to\nschemes:\n- name: HealthieApiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: 'Basic <API_KEY>'\n  required: true\n  description: >-\n    The API key\
  \ is sent in the Authorization header using the literal scheme word \"Basic\" followed by\n    the raw key. Despite the scheme name this is NOT HTTP Basic authentication — the value is the API\n    key itself, not a base64 user:password pair.\n  source: https://docs.gethealthie.com/guides/api-concepts/authentication\n- name: AuthorizationSource\n  type: apiKey\n  in: header\n  parameter_name: AuthorizationSource\n  format: 'API'\n  required: true\n  description: >-\n    Constant discriminator header that must accompany every authenticated API request. Distinguishes\n    API-key traffic from Healthie's own first-party session traffic.\n  source: https://docs.gethealthie.com/guides/api-concepts/authentication\n- name: AuthorizationShard\n  type: apiKey\n  in: header\n  parameter_name: AuthorizationShard\n  format: '<SHARD_AUTHORIZATION_ID>'\n  required: conditional\n  description: >-\n    Required only for customers whose data is hosted in a dedicated Healthie shard. The shard ID is\n  \
  \  not self-service — Healthie issues it on request to hello@gethealthie.com.\n  source: https://docs.gethealthie.com/guides/api-concepts/authentication\n- name: WebsocketToken\n  type: apiKey\n  in: query\n  parameter_name: token\n  format: 'wss://ws.gethealthie.com/subscriptions?token=<API_KEY>'\n  required: true\n  applies_to: GraphQL subscriptions over WebSocket\n  description: >-\n    The WebSocket protocol has no header phase, so Healthie carries the API key as a URL query\n    parameter on the subscription connection. Note the security consequence: a long-lived PHI-bearing\n    credential travels in a URL and is therefore exposed to proxy and connection logs in a way the\n    header-based REST/GraphQL path is not.\n  source: https://docs.gethealthie.com/guides/websockets-and-subscriptions/getting-started/\nscopes:\n  model: account-inherited\n  oauth_scopes: false\n  description: >-\n    Healthie has no OAuth scope surface. An API key is scoped to exactly one Healthie user account\n\
  \    and takes on that account's permissions and behaviours — actions performed with a key are\n    attributed to that user in audit logs and notifications. Access is therefore narrowed by\n    provisioning the underlying user account's role and permissions, not by requesting scopes.\n  patterns:\n  - name: service-account key\n    description: One key tied to a purpose-built admin/service user account. Recommended by Healthie\n      for backend and data-focused integrations.\n  - name: per-user key\n    description: >-\n      A key per end user. Recommended by Healthie when building headless/custom user interfaces, so\n      that audit logging, notifications and defaults mirror how Healthie's own front end behaves.\nkey_management:\n  self_service: partial\n  programmatic_issuance:\n    mutation: createApiKey\n    inputs:\n    - name (optional, user-defined label)\n    - user_id (required)\n    returns:\n    - api_key\n    - 'api_key_object { id, displayable_key, created_at }'\n    -\
  \ 'messages { field, message }'\n    verified_in: graphql/healthie-schema.graphql\n    gate: >-\n      Issuing keys for OTHER users must be enabled by Healthie per account — the docs direct\n      integrators to contact hello@gethealthie.com to have it turned on.\n  listing:\n    queries: [apiKeys, apiKeysCount]\n  multiple_keys_per_account: true\n  rotation_policy_published: false\n  expiry_published: false\ngaps:\n- No OAuth 2.0 or OpenID Connect. Third-party applications cannot obtain delegated, user-consented,\n  scope-limited access to a practice's Healthie data — an integrator holds a full-permission\n  long-lived key instead.\n- No published key rotation or expiry policy, and no documented revocation endpoint beyond the\n  account UI.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server (both 404 — see\n  well-known/healthie-well-known.yml).\n- The API key doubles as the WebSocket credential and is placed in the query string.\nx-evidence:\n  fetched:\
  \ '2026-08-14'\n  urls:\n  - {url: 'https://docs.gethealthie.com/guides/api-concepts/authentication', http_status: 200}\n  - {url: 'https://docs.gethealthie.com/guides/websockets-and-subscriptions/getting-started/', http_status: 200}\n  - {url: 'https://staging-api.gethealthie.com/graphql', http_status: 200, note: introspection confirming createApiKey/ApiKey}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthie/refs/heads/main/authentication/healthie-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- API-First
- Appointments
- Billing
- Care Plans
- Charting
- Claims
- Clinical
- Digital Health
- EHR
- EMR
- Forms
- GraphQL
- Health Tech
- Healthcare
- Insurance
- Intake
- Online Programs
- Patient Engagement
- Patient Portal
- Practice Management
- Programs
- Scheduling
- Telehealth
- Wellness
- Webhooks
---
