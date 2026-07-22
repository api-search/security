---
api_key_in: []
auth_types:
- oauth2
description: The Sugar REST API uses two-legged OAuth 2.0. Clients POST credentials to the per-instance token endpoint and receive an access_token that is sent on subsequent requests in the OAuth-Token request header. Tokens are refreshed with the refresh_token grant. There is no OAuth scope surface - access is governed by Sugar role-based access control (ACLs) on the authenticated user, not by token scopes.
kind: authentication
layout: security
method: searched
name: Sugarcrm Authentication
name_suffix: Authentication
oauth_flows:
- password
- refresh_token
overview: SugarCRM secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and refresh_token flow(s).
provider_name: SugarCRM
provider_slug: sugarcrm
scheme_count: 1
schemes:
- description: Two-legged OAuth 2.0 (Resource Owner Password Credentials + refresh).
  flows:
  - flow: password
    parameters:
      client_id: sugar
      client_secret: ''
      grant_type: password
      password: <password>
      platform: base
      username: <user>
    tokenUrl: https://<site_url>/rest/v11_x/oauth2/token
  - flow: refresh_token
    parameters:
      client_id: sugar
      grant_type: refresh_token
      refresh_token: <refresh_token>
    tokenUrl: https://<site_url>/rest/v11_x/oauth2/token
  name: OAuth2
  request_header: OAuth-Token
  response_fields:
  - access_token
  - refresh_token
  - download_token
  - expires_in
  type: oauth2
slug: sugarcrm-authentication
source_filename: sugarcrm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.sugarcrm.com/documentation/sugar_developer/ (Sugar Developer Guide - REST API / Authentication)\ndocs: https://support.sugarcrm.com/documentation/sugar_developer/sugar_developer_guide_13.0/integration/web_services/rest_api/\ndescription: >-\n  The Sugar REST API uses two-legged OAuth 2.0. Clients POST credentials to the\n  per-instance token endpoint and receive an access_token that is sent on\n  subsequent requests in the OAuth-Token request header. Tokens are refreshed\n  with the refresh_token grant. There is no OAuth scope surface - access is\n  governed by Sugar role-based access control (ACLs) on the authenticated user,\n  not by token scopes.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [password, refresh_token]\n  token_header: OAuth-Token\n  scopes: none\nschemes:\n  - name: OAuth2\n    type: oauth2\n    description: Two-legged OAuth 2.0 (Resource Owner Password Credentials + refresh).\n    flows:\n\
  \      - flow: password\n        tokenUrl: https://<site_url>/rest/v11_x/oauth2/token\n        parameters:\n          grant_type: password\n          client_id: sugar        # default public client; admins may define custom client_ids\n          client_secret: \"\"        # empty by default\n          username: <user>\n          password: <password>\n          platform: base           # customize per integration to avoid session conflicts\n      - flow: refresh_token\n        tokenUrl: https://<site_url>/rest/v11_x/oauth2/token\n        parameters:\n          grant_type: refresh_token\n          client_id: sugar\n          refresh_token: <refresh_token>\n    response_fields: [access_token, refresh_token, download_token, expires_in]\n    request_header: OAuth-Token\nnotes: >-\n  The base URL is instance-specific (https://<site_url>/rest/v{version}/), so\n  the token endpoint and API host vary per Sugar deployment. SSO to Sugar itself\n  supports LDAP, SAML and OIDC, but programmatic REST\
  \ access is via the OAuth2\n  token flow above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sugarcrm/refs/heads/main/authentication/sugarcrm-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Saas
- CRM
- Sales
- Marketing
- Customer Service
- Sales Automation
- REST API
---
