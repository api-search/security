---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sifflet-assets-api-openapi.yml
  format: yaml
  label: Sifflet Assets API
  slug: sifflet-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-assets-api-openapi.yml
- filename: sifflet-calendars-api-openapi.yml
  format: yaml
  label: Sifflet Calendars API
  slug: sifflet-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-calendars-api-openapi.yml
- filename: sifflet-credentials-api-openapi.yml
  format: yaml
  label: Sifflet Credentials API
  slug: sifflet-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-credentials-api-openapi.yml
- filename: sifflet-dbt-integration-api-openapi.yml
  format: yaml
  label: Sifflet dbt integration API
  slug: sifflet-dbt-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-dbt-integration-api-openapi.yml
- filename: sifflet-declarative-assets-and-lineage-api-openapi.yml
  format: yaml
  label: Sifflet Declarative Assets and Lineage API
  slug: sifflet-declarative-assets-and-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-declarative-assets-and-lineage-api-openapi.yml
- filename: sifflet-domains-api-openapi.yml
  format: yaml
  label: Sifflet Domains API
  slug: sifflet-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-domains-api-openapi.yml
- filename: sifflet-external-catalog-api-openapi.yml
  format: yaml
  label: Sifflet External Catalog API
  slug: sifflet-external-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-external-catalog-api-openapi.yml
- filename: sifflet-notification-rules-api-openapi.yml
  format: yaml
  label: Sifflet Notification Rules API
  slug: sifflet-notification-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-notification-rules-api-openapi.yml
- filename: sifflet-rule-api-openapi.yml
  format: yaml
  label: Sifflet Rule API
  slug: sifflet-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-rule-api-openapi.yml
- filename: sifflet-rule-run-api-openapi.yml
  format: yaml
  label: Sifflet Rule Run API
  slug: sifflet-rule-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-rule-run-api-openapi.yml
- filename: sifflet-sources-deprecated-api-openapi.yml
  format: yaml
  label: Sifflet Sources (deprecated) API
  slug: sifflet-sources-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-sources-deprecated-api-openapi.yml
- filename: sifflet-sources-v2-api-openapi.yml
  format: yaml
  label: Sifflet Sources (v2) API
  slug: sifflet-sources-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-sources-v2-api-openapi.yml
- filename: sifflet-teams-api-openapi.yml
  format: yaml
  label: Sifflet Teams API
  slug: sifflet-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-teams-api-openapi.yml
- filename: sifflet-users-api-openapi.yml
  format: yaml
  label: Sifflet Users API
  slug: sifflet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-users-api-openapi.yml
- filename: sifflet-workspace-api-openapi.yml
  format: yaml
  label: Sifflet Workspace API
  slug: sifflet-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/openapi/sifflet-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sifflet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sifflet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sifflet
provider_slug: sifflet
scheme_count: 1
schemes:
- description: All Sifflet public API endpoints require an Access Token passed as a Bearer token. Access Tokens are created in the Sifflet UI under Settings > Access Tokens, are scoped to a role (and optionally to specific domains with a per-domain role), are shown only once at creation, and are valid for 24 months by default (custom expiry configurable). The same Access Token authenticates the API, the CLI, and the Airflow operators.
  name: AccessToken
  scheme: bearer
  sources:
  - https://docs.siffletdata.com/docs/access-tokens.md
  type: http
slug: sifflet-authentication
source_filename: sifflet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.siffletdata.com/docs/access-tokens.md\ndocs: https://docs.siffletdata.com/reference/overview-1.md\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: AccessToken\n    type: http\n    scheme: bearer\n    description: >-\n      All Sifflet public API endpoints require an Access Token passed as a Bearer token.\n      Access Tokens are created in the Sifflet UI under Settings > Access Tokens, are scoped\n      to a role (and optionally to specific domains with a per-domain role), are shown only\n      once at creation, and are valid for 24 months by default (custom expiry configurable).\n      The same Access Token authenticates the API, the CLI, and the Airflow operators.\n    sources: [https://docs.siffletdata.com/docs/access-tokens.md]\nidentity:\n  sso:\n    note: >-\n      Human sign-in to the Sifflet application supports SSO / OpenID Connect via Okta,\n\
  \      Google, Azure Active Directory, and ForgeRock. SSO governs UI login; programmatic API\n      access uses Access Tokens (bearer).\n    docs: https://docs.siffletdata.com/docs/single-sign-on-sso.md\nauthorization:\n  model: role-based\n  note: >-\n    Access Tokens carry a role (Admin, Editor, Viewer, Monitor Responder, Catalog Editor,\n    Domain Editor, etc.) and optional per-domain roles. This is role/permission based rather\n    than OAuth scopes, so no OAuth scope artifact applies.\n  docs: https://docs.siffletdata.com/docs/access-control.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sifflet/refs/heads/main/authentication/sifflet-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Analytics
- Data Observability
- Data Quality
- Data Catalog
- Data Lineage
- Data Governance
- Monitoring
- Metadata
- AI Agents
---
