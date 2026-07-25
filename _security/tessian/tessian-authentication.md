---
api_key_in:
- header
api_specs:
- filename: tessian-anomalies-api-openapi.yml
  format: yaml
  label: Tessian Anomalies API
  slug: tessian-anomalies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-anomalies-api-openapi.yml
- filename: tessian-audits-api-openapi.yml
  format: yaml
  label: Tessian Audits API
  slug: tessian-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-audits-api-openapi.yml
- filename: tessian-beta-endpoints-api-openapi.yml
  format: yaml
  label: Tessian Beta Endpoints API
  slug: tessian-beta-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-beta-endpoints-api-openapi.yml
- filename: tessian-deprecated-api-openapi.yml
  format: yaml
  label: Tessian Deprecated API
  slug: tessian-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-deprecated-api-openapi.yml
- filename: tessian-endpoints-api-openapi.yml
  format: yaml
  label: Tessian Endpoints API
  slug: tessian-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-endpoints-api-openapi.yml
- filename: tessian-events-api-openapi.yml
  format: yaml
  label: Tessian Events API
  slug: tessian-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-events-api-openapi.yml
- filename: tessian-groups-api-openapi.yml
  format: yaml
  label: Tessian Groups API
  slug: tessian-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-groups-api-openapi.yml
- filename: tessian-monitoring-api-openapi.yml
  format: yaml
  label: Tessian Monitoring API
  slug: tessian-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-monitoring-api-openapi.yml
- filename: tessian-risk-api-openapi.yml
  format: yaml
  label: Tessian Risk API
  slug: tessian-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-risk-api-openapi.yml
- filename: tessian-triggers-api-openapi.yml
  format: yaml
  label: Tessian Triggers API
  slug: tessian-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-triggers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tessian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tessian secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tessian
provider_slug: tessian
scheme_count: 1
schemes:
- description: A Tessian portal user with "Logs" permission generates an API Token under Integrations > Tessian API in the portal. The token is shown only once at creation. It inherits the permissions of the creating user and is automatically revoked if that user is removed or loses the Logs permission, or when the token is deleted.
  format: 'Authorization: API-Token <your-api-token>'
  header_name: Authorization
  in: header
  name: api-token
  sources:
  - openapi/tessian-openapi-original.json
  type: apiKey
slug: tessian-authentication
source_filename: tessian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.tessian.com/documentation/api/index.html\ndocs: https://developer.tessian.com/documentation/api/index.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The Tessian API uses a static API Token passed in the Authorization header.\n    The OpenAPI document does not declare a components.securitySchemes entry;\n    this profile is captured from the provider's published authentication docs.\nschemes:\n- name: api-token\n  type: apiKey\n  in: header\n  header_name: Authorization\n  format: 'Authorization: API-Token <your-api-token>'\n  sources:\n  - openapi/tessian-openapi-original.json\n  description: >-\n    A Tessian portal user with \"Logs\" permission generates an API Token under\n    Integrations > Tessian API in the portal. The token is shown only once at\n    creation. It inherits the permissions of the creating user and is\n    automatically revoked if that\
  \ user is removed or loses the Logs permission,\n    or when the token is deleted.\ntoken_lifecycle:\n  shown_once: true\n  inherits_user_permissions: true\n  required_permission: Logs\n  auto_revoked_when:\n  - user removed\n  - Logs permission revoked\n  - token deleted\n  system_account_supported: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/authentication/tessian-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Email Security
- Cybersecurity
- Data Loss Prevention
- SIEM
- Security
- Phishing
---
