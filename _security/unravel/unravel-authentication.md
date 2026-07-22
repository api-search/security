---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Unravel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unravel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unravel
provider_slug: unravel
scheme_count: 1
schemes:
- description: 'API authorization token created in the Unravel UI, required while interacting with Unravel APIs. Requests send the token in an Authorization header with the JWT prefix (documented request examples use -H "Authorization: JWT <token>"). Roles are Admin or User; User tokens can be scoped with RBAC tags.'
  header: 'Authorization: JWT <token>'
  in: header
  jwt_secret_rotation: https://docs.unraveldata.com/unravel-v482x/en/jwt-rotate.html
  name: apiToken
  persistence: Deleted on server restart unless com.unraveldata.api.access.tokens.store is configured to a persistent JSON token store.
  roles:
  - Admin
  - User
  type: apiKey
slug: unravel-authentication
source_filename: unravel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.unraveldata.com/unravel-v482x/en/api-token.html\ndocs: https://docs.unraveldata.com/unravel-v482x/en/api-token.html\nsummary:\n  types: [apiKey]\n  model: api-token\n  notes: Unravel's REST APIs are authorized with API tokens. An administrator creates\n    tokens from the Unravel UI (Manage > API Tokens) with a Client Id and a role\n    (Admin or User; User tokens can carry RBAC tags). Tokens are backed by a JSON\n    web token (JWT) secret that can be rotated. By default tokens are deleted when\n    the Unravel server restarts; persistent tokens require setting the\n    com.unraveldata.api.access.tokens.store property to a JSON token store file.\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: header\n    header: 'Authorization: JWT <token>'\n    description: >-\n      API authorization token created in the Unravel UI, required while\n      interacting with Unravel APIs. Requests send the token in an Authorization\n\
  \      header with the JWT prefix (documented request examples use\n      -H \"Authorization: JWT <token>\"). Roles are Admin or User; User tokens can\n      be scoped with RBAC tags.\n    roles: [Admin, User]\n    persistence: Deleted on server restart unless com.unraveldata.api.access.tokens.store\n      is configured to a persistent JSON token store.\n    jwt_secret_rotation: https://docs.unraveldata.com/unravel-v482x/en/jwt-rotate.html\nui_authentication:\n  - LDAP (Enabling LDAP authentication for Unravel UI)\n  - SAML (Enabling SAML Authentication for Unravel User; Azure AD, Okta via Auth0)\n  - Kerberos (Configuring Kerberos for secure cluster access)\n  - Role-Based Access Control (RBAC) with role types and user tags\nnotes: Unravel is a self-hosted / SaaS data observability platform; the REST API is\n  served by the customer's Unravel instance rather than a single public cloud host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unravel/refs/heads/main/authentication/unravel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Observability
- FinOps
- DataOps
- Cost Optimization
- Databricks
- Snowflake
- BigQuery
- Monitoring
- Company
---
