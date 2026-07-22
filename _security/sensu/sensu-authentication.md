---
api_key_in:
- header
auth_types:
- http
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Sensu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sensu secures its APIs with http, apiKey, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sensu
provider_slug: sensu
scheme_count: 3
schemes:
- description: 'Obtain a JWT access token by POSTing credentials to the /auth endpoint. Access tokens are short-lived (~15 minutes) and are refreshed via /auth/token using the accompanying refresh token. Presented as Authorization: Bearer <token>.'
  name: JWT Access Token
  refresh_url: /auth/token
  scheme: bearer
  token_url: /auth
  ttl: ~15m
  type: http
- description: 'Persistent API keys are UUIDs mapped to a Sensu username, created via the core/v2 apikeys resource. Presented as Authorization: Key <uuid> and do not expire on the 15-minute token cycle.'
  example: 'Authorization: Key 7f63b5bc-41f4-4b3e-b59b-5431afd7e6a2'
  format: Key <uuid>
  in: header
  name: API Key
  parameter_name: Authorization
  type: apiKey
- description: Operators can authenticate to the backend and sensuctl via OIDC providers (e.g. Microsoft Entra ID) for single sign-on. Configured as a Sensu auth provider resource.
  name: OIDC Single Sign-On
  type: openIdConnect
slug: sensu-authentication
source_filename: sensu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sensu.io/sensu-go/latest/api/\ndocs: https://docs.sensu.io/sensu-go/latest/api/#authenticate-with-the-authentication-api\nsummary:\n  types: [http, apiKey, openIdConnect]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  oidc: true\n  rbac: true\n  unauthenticated_endpoints: [/auth, /health, /license, /metrics, /ready, /version]\nschemes:\n- name: JWT Access Token\n  type: http\n  scheme: bearer\n  description: >-\n    Obtain a JWT access token by POSTing credentials to the /auth endpoint. Access\n    tokens are short-lived (~15 minutes) and are refreshed via /auth/token using the\n    accompanying refresh token. Presented as Authorization: Bearer <token>.\n  token_url: /auth\n  refresh_url: /auth/token\n  ttl: ~15m\n- name: API Key\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: 'Key <uuid>'\n  description: >-\n    Persistent API keys are UUIDs mapped to a Sensu username, created via\
  \ the\n    core/v2 apikeys resource. Presented as Authorization: Key <uuid> and do not\n    expire on the 15-minute token cycle.\n  example: 'Authorization: Key 7f63b5bc-41f4-4b3e-b59b-5431afd7e6a2'\n- name: OIDC Single Sign-On\n  type: openIdConnect\n  description: >-\n    Operators can authenticate to the backend and sensuctl via OIDC providers\n    (e.g. Microsoft Entra ID) for single sign-on. Configured as a Sensu auth\n    provider resource.\nauthorization:\n  model: RBAC\n  description: >-\n    Access is governed by role-based access control: roles / cluster roles define\n    verbs on resource types, bound to users or groups via role bindings /\n    cluster role bindings, scoped by namespace. Sensu uses RBAC rather than OAuth2\n    scopes, so no OAuth scope reference exists (scopes/ artifact intentionally omitted).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensu/refs/heads/main/authentication/sensu-authentication.yml
summary_line: http/apiKey/openIdConnect · 3 schemes
tags:
- Company
- Monitoring
- Observability
- Infrastructure
- DevOps
- Metrics
- Events
- Alerting
- Monitoring as Code
- Kubernetes
---
