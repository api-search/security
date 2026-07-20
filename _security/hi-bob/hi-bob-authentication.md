---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hi Bob Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hi Bob secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hi Bob
provider_slug: hi-bob
scheme_count: 2
schemes:
- description: 'Token-based auth using an API "service user". Combine the service user ID and token into a single "id:token" string, Base64-encode it, and send it as "Authorization: Basic <encoded>". Service users are not tied to a real employee and have no access by default — permissions are granted per category/field via a permission group (view / edit / history + access rights on which employees).'
  docs: https://apidocs.hibob.com/docs/api-service-users
  name: ServiceUserBasic
  scheme: basic
  type: http
- description: OAuth 2.0 for approved Marketplace / technology partners. Customers install the app from the Bob Marketplace or a partner landing page; consent is granted in HiBob and the partner receives client_id / client_secret plus access + refresh tokens. Scopes map to specific endpoints (see scopes/hi-bob-scopes.yml).
  docs: https://apidocs.hibob.com/reference/oauth-20
  flows:
  - authorizationUrl: https://auth.app.hibob.com/
    flow: authorizationCode
    refreshUrl: https://auth.app.hibob.com/oauth2/v1/apps/token
    tokenUrl: https://auth.app.hibob.com/oauth2/v1/apps/token
  name: OAuth2
  type: oauth2
slug: hi-bob-authentication
source_filename: hi-bob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apidocs.hibob.com/reference/authorization\ndocs: https://apidocs.hibob.com/docs/api-service-users\nsummary:\n  types: [http, oauth2]\n  http_schemes: [basic]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Direct API integrations authenticate with a service user (HTTP Basic). Approved\n    HiBob Marketplace / technology partners use OAuth 2.0 (authorization code +\n    refresh) scoped to endpoint-level permissions.\nschemes:\n- name: ServiceUserBasic\n  type: http\n  scheme: basic\n  description: >-\n    Token-based auth using an API \"service user\". Combine the service user ID and\n    token into a single \"id:token\" string, Base64-encode it, and send it as\n    \"Authorization: Basic <encoded>\". Service users are not tied to a real employee\n    and have no access by default — permissions are granted per category/field via a\n    permission group (view / edit / history + access rights on which employees).\n\
  \  docs: https://apidocs.hibob.com/docs/api-service-users\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 for approved Marketplace / technology partners. Customers install the\n    app from the Bob Marketplace or a partner landing page; consent is granted in\n    HiBob and the partner receives client_id / client_secret plus access + refresh\n    tokens. Scopes map to specific endpoints (see scopes/hi-bob-scopes.yml).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.app.hibob.com/\n    tokenUrl: https://auth.app.hibob.com/oauth2/v1/apps/token\n    refreshUrl: https://auth.app.hibob.com/oauth2/v1/apps/token\n  docs: https://apidocs.hibob.com/reference/oauth-20\ndeprecated:\n- name: API Access Tokens\n  status: deprecated\n  replaced_by: ServiceUserBasic\n  docs: https://apidocs.hibob.com/docs/transition-from-api-access-tokens\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hi-bob/refs/heads/main/authentication/hi-bob-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- HR
- HRIS
- Human Resources
- Payroll
- People Analytics
- Time Off
- Workforce Planning
- Employees
- HR Tech
---
