---
api_key_in: []
auth_types:
- sessionToken
description: ''
kind: authentication
layout: security
method: searched
name: Unravel Data Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unravel Data Systems secures its APIs with sessionToken across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Unravel Data Systems
provider_slug: unravel-data-systems
scheme_count: 2
schemes:
- description: Authenticate with POST /signIn against the deployment's API base (https://unravel-host:3000/api/v1). The Unravel server returns a session token which must be included in all subsequent requests. Access level is determined by the caller's RBAC role. All requests and responses are JSON over HTTP or HTTPS.
  name: signInSessionToken
  type: apiKey
- description: The Unravel web UI (not the REST API) supports LDAP authentication and SAML single sign-on, configured per deployment; JSON web token (JWT) secrets used by the platform can be rotated by administrators.
  name: webUiSso
  scope: web-ui
  type: enterprise-sso
slug: unravel-data-systems-authentication
source_filename: unravel-data-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  http://unravel-docs.unraveldata.com/unravel-v4823x/en/on-prem-apis.html\n  (Unravel REST APIs documentation) — no machine-readable OpenAPI is published,\n  so this profile is taken from the docs rather than derived from\n  securitySchemes.\ndocs: http://unravel-docs.unraveldata.com/unravel-v4823x/en/on-prem-apis.html\nsummary:\n  types: [sessionToken]\n  oauth2_flows: []\n  notes: Session-token authentication; no OAuth2/OIDC surface on the product API.\nschemes:\n  - name: signInSessionToken\n    type: apiKey\n    description: >-\n      Authenticate with POST /signIn against the deployment's API base\n      (https://unravel-host:3000/api/v1). The Unravel server returns a session\n      token which must be included in all subsequent requests. Access level is\n      determined by the caller's RBAC role. All requests and responses are\n      JSON over HTTP or HTTPS.\n  - name: webUiSso\n    type: enterprise-sso\n    description:\
  \ >-\n      The Unravel web UI (not the REST API) supports LDAP authentication and\n      SAML single sign-on, configured per deployment; JSON web token (JWT)\n      secrets used by the platform can be rotated by administrators.\n    scope: web-ui\nrbac:\n  supported: true\n  notes: >-\n    Role-based access control with role types and user tags; API access level\n    follows the authenticated user's RBAC role.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unravel-data-systems/refs/heads/main/authentication/unravel-data-systems-authentication.yml
summary_line: sessionToken · 2 schemes
tags:
- Data Observability
- FinOps
- DataOps
- Databricks
- Snowflake
- BigQuery
- Cost Optimization
- Performance
---
