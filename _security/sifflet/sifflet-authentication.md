---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
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
