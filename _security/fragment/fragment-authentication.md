---
api_key_in: []
auth_types:
- oauth2
description: 'Fragment authenticates API requests with the OAuth2 client-credentials flow. You create an API client (client_id + client_secret) in the Fragment dashboard, exchange those credentials for a short-lived Bearer access token at a region-specific token endpoint, and send it as `Authorization: Bearer <access_token>` on GraphQL requests. Access tokens expire after one hour. Identity is brokered through Auth0 (idp.fragment.dev) with the API audience https://api-global.fragment.dev.'
kind: authentication
layout: security
method: searched
name: Fragment Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Fragment secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Fragment
provider_slug: fragment
scheme_count: 1
schemes:
- audience: https://api-global.fragment.dev
  flow: clientCredentials
  header: 'Authorization: Bearer <access_token>'
  idp: idp.fragment.dev
  name: OAuth2ClientCredentials
  scope_param: true
  sources:
  - https://fragment.dev/api-reference/ledger-overview
  token_url_pattern: https://auth.<region>.fragment.dev/oauth2/token
  type: oauth2
slug: fragment-authentication
source_filename: fragment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://fragment.dev/docs/authenticate-with-the-api\ndocs: https://fragment.dev/api-reference/ledger-overview\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\n  token_ttl_seconds: 3600\ndescription: >-\n  Fragment authenticates API requests with the OAuth2 client-credentials flow.\n  You create an API client (client_id + client_secret) in the Fragment\n  dashboard, exchange those credentials for a short-lived Bearer access token\n  at a region-specific token endpoint, and send it as `Authorization: Bearer\n  <access_token>` on GraphQL requests. Access tokens expire after one hour.\n  Identity is brokered through Auth0 (idp.fragment.dev) with the API audience\n  https://api-global.fragment.dev.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url_pattern: https://auth.<region>.fragment.dev/oauth2/token\n  audience: https://api-global.fragment.dev\n\
  \  idp: idp.fragment.dev\n  header: 'Authorization: Bearer <access_token>'\n  scope_param: true\n  sources: [https://fragment.dev/api-reference/ledger-overview]\ntoken_endpoints:\n- https://auth.ap-southeast-2.fragment.dev/oauth2/token\n- https://auth.us-east-1.fragment.dev/oauth2/token\n- https://auth.us-east-2.fragment.dev/oauth2/token\n- https://auth.us-west-2.fragment.dev/oauth2/token\n- https://auth.eu-west-1.fragment.dev/oauth2/token\nnotes:\n- API clients (client_id/client_secret) are provisioned per workspace in the dashboard.\n- Roles & Permissions (Admin / Reader) can be assigned to API clients (changelog, June 2026).\n- No scope reference page was published at the time of capture; scopes are requested via the OAuth `scope` parameter.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fragment/refs/heads/main/authentication/fragment-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ledger
- Accounting
- Payments
- Fintech
- Double-Entry
- Money Movement
- GraphQL
- Financial Infrastructure
- Reconciliation
---
