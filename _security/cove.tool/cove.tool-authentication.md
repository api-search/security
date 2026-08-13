---
api_key_in:
- header
api_specs:
- filename: cove.tool-rest-api-v2-openapi.yml
  format: yaml
  label: cove.tool REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-rest-api-v2-openapi.yml
- filename: cove.tool-api-v1-openapi.yml
  format: yaml
  label: cove.tool API v1
  slug: api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-api-v1-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cove.Tool Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cove.Tool secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cove.Tool
provider_slug: cove.tool
scheme_count: 2
schemes:
- format: Token <api_token>
  in: header
  name: AuthToken
  note: Named `AuthToken` in v1 and `apiKeyAuth` in v2 — same mechanism, renamed across the version boundary with no note in either document.
  parameter: Authorization
  sources:
  - openapi/cove.tool-api-v1-openapi.yml
  - openapi/cove.tool-rest-api-v2-openapi.yml
  type: apiKey
- format: Token <api_token>
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/cove.tool-rest-api-v2-openapi.yml
  type: apiKey
slug: cove.tool-authentication
source_filename: cove.tool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: >-\n  openapi/cove.tool-rest-api-v2-openapi.yml, openapi/cove.tool-api-v1-openapi.yml,\n  https://developers.covetool.com/ (info.description Authentication section),\n  live 401 from https://app.covetool.com/api/v2/energy-codes\ndocs: https://developers.covetool.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  oidc: false\n  mtls: false\n  basic: false\n  bearer: false\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token <api_token>'\n  sources:\n  - openapi/cove.tool-api-v1-openapi.yml\n  - openapi/cove.tool-rest-api-v2-openapi.yml\n  note: >-\n    Named `AuthToken` in v1 and `apiKeyAuth` in v2 — same mechanism, renamed across the version\n    boundary with no note in either document.\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token <api_token>'\n  sources:\n  - openapi/cove.tool-rest-api-v2-openapi.yml\n\
  token_issuance:\n  endpoint: https://app.covetool.com/api/get-token\n  method: POST\n  documented_in: 'OpenAPI info.description, \"Generating an API Token\" table'\n  v1_operation: 'POST /get-token'\n  probed_status: 405\n  probed_note: >-\n    A GET on /api/get-token returns 405, confirming POST-only. The credential exchange itself was\n    not exercised — it requires real account credentials, and this pipeline uses none.\n  prerequisite: 'A valid trial or licensed cove.tool account. There is no self-serve API tier.'\nobserved:\n  method: probed\n  url: https://app.covetool.com/api/v2/energy-codes\n  status: 401\n  www_authenticate: Token\n  body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n  note: >-\n    Django REST Framework TokenAuthentication. The challenge scheme is `Token`, NOT RFC 6750\n    `Bearer` — a client that sends `Authorization: Bearer <t>` will be rejected. This distinction is\n    easy to miss because the v2 spec models the scheme as a generic `apiKey`\
  \ in the `Authorization`\n    header without stating the prefix; the prefix is only visible on the wire and in the\n    description's examples.\nunauthenticated_operations:\n- operation: 'POST /auth/signup'\n  spec: openapi/cove.tool-rest-api-v2-openapi.yml\n  note: >-\n    Declares no `security` and is therefore anonymous, yet it creates a user account against an\n    organization's cove.tool license. This is the sharpest edge on the auth surface and it is not\n    called out in the documentation.\nscopes:\n  supported: false\n  note: >-\n    No OAuth2, no scopes, no permission strings. Authorization is coarse: a token acts as its\n    profile, and access is bounded by the business the profile belongs to — a cross-business\n    profile read returns 403. `is_owner` and `is_admin` on the profile are the only role signals,\n    and neither is settable through the API. No scopes/ artifact was written because there is\n    nothing to derive; derive-oauth-scopes.py returned zero oauth2 schemes.\n\
  rotation:\n  documented: false\n  note: 'No token expiry, rotation, revocation or refresh guidance published.'\ntransport_security:\n  https_required: true\n  hsts: false\n  note: 'TLS 1.2 on app.covetool.com; strict-transport-security is not set. See security/cove.tool-domain-security.yml.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/authentication/cove.tool-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Building Performance
- Energy Modeling
- Daylight Analysis
- Sustainability
- Architecture
- AEC
- Simulation
- Embodied Carbon
- Building Design
---
