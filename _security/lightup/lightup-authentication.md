---
api_key_in: []
api_specs:
- filename: lightup-dashboard-openapi.json
  format: json
  label: Lightup Dashboard API
  slug: dashboard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-dashboard-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Lightup Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightup secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lightup
provider_slug: lightup
scheme_count: 1
schemes:
- applied_to_operations: 52
  bearerFormat: JWT
  in: header
  name: bearerAuth
  parameter_name: authorization
  scheme: bearer
  sources:
  - openapi/lightup-dashboard-openapi.json
  type: http
  value_format: Bearer <access-token>
slug: lightup-authentication
source_filename: lightup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.lightup.ai/reference/post_api-v1-token-refresh\ndocs: https://docs.lightup.ai/docs/api-credentials\nderive_note: The published OpenAPI declares no components.securitySchemes. Authorization\n  is modelled as an explicit `authorization` header parameter on 52 of the 54 operations,\n  so this profile was authored from the documented credential flow rather than derived\n  mechanically.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  scopes_published: false\n  model: JWT bearer access token, obtained by exchanging a long-lived refresh token\n    from a downloaded API credential file.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter_name: authorization\n  value_format: Bearer <access-token>\n  applied_to_operations: 52\n  sources:\n  - openapi/lightup-dashboard-openapi.json\ntoken_flow:\n  credential_file:\n    description: Generated\
  \ in the Lightup app under the gear icon -> API Credentials\n      -> Generate API credential, then downloaded as a JSON file.\n    filename_pattern: lightup-api-credential*.json\n    contains:\n    - refresh token\n    - host / cluster URL\n  exchange:\n    operation: POST /api/v1/token/refresh/\n    docs: https://docs.lightup.ai/reference/post_api-v1-token-refresh\n    request_field: refresh\n    response_field: access\n    description: >-\n      Exchange the refresh value from the credential file for a short-lived access\n      token, then send it in the Authorization header as \"Bearer <access>\" on\n      subsequent calls.\n  cluster_scoping: Credentials are bound to a specific Lightup cluster; requests must\n    target the matching https://app.<clusterId>.lightup.ai host.\nconsumers:\n- name: lightctl CLI\n  credential_path: ~/.lightup/credential\n  env: LIGHTCTL_CREDENTIAL_PATH\n- name: Lightup MCP server\n  description: Connects as /sse?host=<instance>&refresh_token=<JWT refresh\
  \ token>;\n    stateless, credentials never stored server-side.\nauthorization:\n  model: role-based access control\n  docs: https://docs.lightup.ai/docs/roles\n  app_roles:\n  - name: App Admin\n    description: Invite users, set app roles, create workspaces, invite users to workspaces\n      and set their initial workspace role.\n  - name: App Editor\n    description: Create workspaces, but cannot invite new app users or set app roles.\n  - name: App Viewer\n    description: Can be invited to join any workspace, but cannot create workspaces.\n  workspace_roles:\n  - name: Admin\n    description: Everything associated with creating, editing and operationalizing\n      metrics and monitors, including managing datasources.\n  - name: Editor\n    description: Everything Admins can do except managing datasources.\n  - name: Viewer\n    description: Read access to workspace objects.\n  - name: Observer\n    description: Most restricted workspace role; includes table sample preview permissions\n\
  \      added in release 4.21.\n  scoping: Most API resources are workspace-scoped via a {workspace_id} path segment;\n    a 403 is returned when the user lacks access to the workspace.\nsso:\n  cloud:\n  - Google SSO\n  - Okta\n  enterprise:\n  - Google SSO\n  - Okta\n  - SAML\n  - Microsoft AD\n  source: https://www.lightup.ai/pricing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/authentication/lightup-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Quality
- Data Observability
- Data Monitoring
- Anomaly Detection
- Data Engineering
- Analytics
- Incident Management
- Artificial Intelligence
- Data Governance
- Company
---
