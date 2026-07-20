---
api_key_in:
- header
api_specs:
- filename: cloud-ops-api.yml
  format: yaml
  label: Temporal Cloud Ops API
  slug: cloud-ops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/openapi/cloud-ops-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Temporal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Temporal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Temporal
provider_slug: temporal
scheme_count: 1
schemes:
- bearerFormat: API Key
  docs: https://docs.temporal.io/cloud/api-keys
  header: Authorization
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cloud-ops-api.yml
  type: http
  value: Bearer <API_KEY>
slug: temporal-authentication
source_filename: temporal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/cloud-ops-api.yml\ndocs: https://docs.temporal.io/cloud/api-keys\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in:\n  - header\n  authorization: rbac\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  header: Authorization\n  value: \"Bearer <API_KEY>\"\n  docs: https://docs.temporal.io/cloud/api-keys\n  sources:\n  - openapi/cloud-ops-api.yml\nauthorization:\n  model: rbac\n  docs: https://docs.temporal.io/cloud/users\n  account_roles:\n    - {role: Account Owner, description: Full account administration access.}\n    - {role: Account Admin, description: Manage namespaces, users, and service accounts.}\n    - {role: Account Developer, description: Create namespaces and manage Nexus endpoints.}\n    - {role: Finance Admin, description: View usage and billing information.}\n    - {role: Account Read, description: Read-only access to account resources.}\n\
  \  namespace_roles:\n    - {role: Namespace Admin, description: Full access to namespace configuration and data.}\n    - {role: Namespace Write, description: Execute workflows and modify workflow data.}\n    - {role: Namespace Read, description: Read-only access to namespace data.}\n  note: >-\n    Each Cloud Ops operation requires a valid API key plus the appropriate\n    account- or namespace-level role. Namespace roles are scoped per namespace.\ndata_plane_note: >-\n  The Temporal Workflow (data-plane) API and self-hosted server authenticate\n  namespace connections with mutual TLS (mTLS) client certificates or, on\n  Temporal Cloud, API keys; the Cloud Ops control-plane API uses API-key bearer\n  auth only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/authentication/temporal-authentication.yml
summary_line: http · 1 scheme
tags:
- ProCode_API_Composition
- Workflows
---
