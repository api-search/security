---
api_key_in:
- header
api_specs:
- filename: picus-security-activity-logs-api-openapi.yml
  format: yaml
  label: Picus Security Activity Logs API
  slug: picus-security-activity-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-activity-logs-api-openapi.yml
- filename: picus-security-agents-api-openapi.yml
  format: yaml
  label: Picus Security Agents API
  slug: picus-security-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-agents-api-openapi.yml
- filename: picus-security-authentication-api-openapi.yml
  format: yaml
  label: Picus Security Authentication API
  slug: picus-security-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-authentication-api-openapi.yml
- filename: picus-security-instances-api-openapi.yml
  format: yaml
  label: Picus Security Instances API
  slug: picus-security-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-instances-api-openapi.yml
- filename: picus-security-integrations-api-openapi.yml
  format: yaml
  label: Picus Security Integrations API
  slug: picus-security-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-integrations-api-openapi.yml
- filename: picus-security-mitigation-api-openapi.yml
  format: yaml
  label: Picus Security Mitigation API
  slug: picus-security-mitigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-mitigation-api-openapi.yml
- filename: picus-security-simulation-latest-result-api-openapi.yml
  format: yaml
  label: Picus Security Simulation Latest Result API
  slug: picus-security-simulation-latest-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-simulation-latest-result-api-openapi.yml
- filename: picus-security-simulation-result-api-openapi.yml
  format: yaml
  label: Picus Security Simulation Result API
  slug: picus-security-simulation-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-simulation-result-api-openapi.yml
- filename: picus-security-simulation-result-reports-api-openapi.yml
  format: yaml
  label: Picus Security Simulation Result Reports API
  slug: picus-security-simulation-result-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-simulation-result-reports-api-openapi.yml
- filename: picus-security-simulations-api-openapi.yml
  format: yaml
  label: Picus Security Simulations API
  slug: picus-security-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-simulations-api-openapi.yml
- filename: picus-security-summary-api-openapi.yml
  format: yaml
  label: Picus Security Summary API
  slug: picus-security-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-summary-api-openapi.yml
- filename: picus-security-templates-api-openapi.yml
  format: yaml
  label: Picus Security Templates API
  slug: picus-security-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-templates-api-openapi.yml
- filename: picus-security-threats-api-openapi.yml
  format: yaml
  label: Picus Security Threats API
  slug: picus-security-threats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-threats-api-openapi.yml
- filename: picus-security-users-api-openapi.yml
  format: yaml
  label: Picus Security Users API
  slug: picus-security-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/openapi/picus-security-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Picus Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Picus Security secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Picus Security
provider_slug: picus-security
scheme_count: 1
schemes:
- applied: global
  applied_note: Declared as a global `security` requirement on the root document and repeated per operation.
  description: After getting the access token, type "Bearer accessToken" in the Authorization header value to request access to the endpoints.
  in: header
  name: Access-Token
  parameter: Authorization
  sources:
  - openapi/picus-security-activity-logs-openapi.yml
  - openapi/picus-security-agents-openapi.yml
  - openapi/picus-security-authentication-openapi.yml
  - openapi/picus-security-instances-openapi.yml
  - openapi/picus-security-integrations-openapi.yml
  - openapi/picus-security-mitigation-openapi.yml
  - openapi/picus-security-simulation-latest-result-openapi.yml
  - openapi/picus-security-simulation-result-openapi.yml
  - openapi/picus-security-simulation-result-reports-openapi.yml
  - openapi/picus-security-simulations-openapi.yml
  - openapi/picus-security-summary-openapi.yml
  - openapi/picus-security-templates-openapi.yml
  - openapi/picus-security-threats-openapi.yml
  - openapi/picus-security-users-openapi.yml
  type: apiKey
  value_form: Bearer {accessToken}
slug: picus-security-authentication
source_filename: picus-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\ndocs: https://apidocs.picussecurity.com/docs/authentication-method\nsource: >-\n  https://apidocs.picussecurity.com/docs/authentication-method (upgraded a derived pass over the 14\n  openapi/ spec files split from openapi/_original/picus-security-openapi.json)\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: refresh-token-exchange\n  note: >-\n    Picus describes the model as OAuth2 (\"OAuth2 protocol is used to authorize Refresh/Access tokens\") but\n    the contract declares a single apiKey scheme and the exchange is a proprietary JSON POST, not an\n    RFC 6749 token endpoint. See conformance/picus-security-conformance.yml.\nflow:\n  step_1:\n    action: Generate a refresh token (human, in the console)\n    where: app.picussecurity.com > Settings > Rest API Token > Generate Token\n    inputs: [token name (unique), description, expiration in days, scope]\n    ttl: 6 months\n    note: >-\n      The token and its\
  \ curl command are displayed exactly once and cannot be retrieved afterwards. The\n      console lists existing tokens with name, creation date, created by, expiration date, scopes and\n      active/expired status.\n  step_2:\n    action: Exchange the refresh token for an access token\n    operationId: AuthTokenParam\n    request: POST https://api.picussecurity.com/v1/auth/token\n    request_headers:\n      Content-Type: application/json\n    request_body: '{\"refresh_token\": \"<refresh token>\"}'\n    response_body: '{\"token\": \"<access token>\", \"expire_at\": <unix epoch MILLISECONDS>}'\n    ttl: 2 hours\n    unauthenticated: true\n  step_3:\n    action: Call any endpoint with the access token\n    header: 'Authorization: Bearer <accessToken>'\n    note: All Picus API endpoints except the token endpoint use this single credential.\n  rotation:\n    action: Regenerate the refresh token\n    operationId: RegenerateRefreshTokenParam\n    request: POST https://api.picussecurity.com/v1/auth/refresh\n\
  \    effect: >-\n      Issues a new refresh token and INVALIDATES the previous refresh and access tokens. Cannot be used once\n      the refresh token has already expired — a new one must then be generated from the console.\nscopes:\n  supported: true\n  published: false\n  note: >-\n    Refresh tokens are created with a SCOPE that \"is used to filter the API endpoints accessible by the\n    token\", and the console shows a scopes column per token. Picus does not publish the scope vocabulary in\n    the docs or declare it in the contract, so no scopes/ artifact can be captured. A 403 on an endpoint the\n    user's role permits usually means the token's scope is too narrow.\nauthorization:\n  model: role-based\n  roles_endpoint: GET /v1/users/roles (RolesFilterParams)\n  assign_endpoint: PUT /v1/users/{userId}/role (assignRoleParams)\n  note: >-\n    Effective permission is the intersection of the user's assigned role and the refresh token's scope.\nschemes:\n- name: Access-Token\n  type:\
  \ apiKey\n  in: header\n  parameter: Authorization\n  value_form: 'Bearer {accessToken}'\n  applied: global\n  applied_note: Declared as a global `security` requirement on the root document and repeated per operation.\n  description: >-\n    After getting the access token, type \"Bearer accessToken\" in the Authorization header value to request\n    access to the endpoints.\n  sources:\n  - openapi/picus-security-activity-logs-openapi.yml\n  - openapi/picus-security-agents-openapi.yml\n  - openapi/picus-security-authentication-openapi.yml\n  - openapi/picus-security-instances-openapi.yml\n  - openapi/picus-security-integrations-openapi.yml\n  - openapi/picus-security-mitigation-openapi.yml\n  - openapi/picus-security-simulation-latest-result-openapi.yml\n  - openapi/picus-security-simulation-result-openapi.yml\n  - openapi/picus-security-simulation-result-reports-openapi.yml\n  - openapi/picus-security-simulations-openapi.yml\n  - openapi/picus-security-summary-openapi.yml\n  - openapi/picus-security-templates-openapi.yml\n\
  \  - openapi/picus-security-threats-openapi.yml\n  - openapi/picus-security-users-openapi.yml\ngaps:\n- No OIDC discovery document and no RFC 8414 authorization-server metadata (all /.well-known/ paths 404).\n- No mTLS, no client credentials, no PKCE — the refresh token is a bearer secret with a 6 month lifetime.\n- The scope vocabulary is enforced but unpublished, so token least-privilege cannot be planned from the docs.\n- The expire_at field is milliseconds while the rate-limit reset header is seconds — an easy client bug.\nevidence:\n- url: https://apidocs.picussecurity.com/docs/authentication-method\n  http_status: 200\n  fetched: '2026-08-02'\n- source: openapi/_original/picus-security-openapi.json\n  kind: securityDefinitions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picus-security/refs/heads/main/authentication/picus-security-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cybersecurity
- Security Validation
- Breach and Attack Simulation
- Adversarial Exposure Validation
- Continuous Threat Exposure Management
- Penetration Testing
- Threat Intelligence
- mitre-attack
- Detection Engineering
- Security Operations
---
