---
api_key_in: []
auth_types:
- oauth2
- http-basic
description: 'The Toshl API supports two authentication methods: OAuth 2.0 bearer tokens (authorization code and implicit grants; user-revocable) and HTTP Basic authentication using long-lived personal tokens created in the Toshl account settings (apps section, available since 26 April 2016). Access tokens default to a 3600-second lifetime with refresh tokens for renewal; refresh tokens can be revoked by users or Toshl staff at any time. Client registration (client_id and client_secret) is required before using OAuth.

  '
kind: authentication
layout: security
method: searched
name: Toshl Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Toshl secures its APIs with oauth2 and http-basic across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Toshl
provider_slug: toshl
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://toshl.com/oauth2/authorize
    flow: authorizationCode
    notes: Authorization code is valid for 30 seconds; token endpoint uses HTTP Basic auth with client credentials
    tokenUrl: https://toshl.com/oauth2/token
  - authorizationUrl: https://toshl.com/oauth2/authorize
    flow: implicit
    notes: For insecure clients; returns a token directly after user approval
  name: OAuth2
  refresh_tokens: true
  scopes_docs: https://developer.toshl.com/docs/oauth
  token_lifetime_seconds: 3600
  type: oauth2
- name: PersonalToken
  notes: Long-lived personal tokens generated in Toshl account settings, used via HTTP Basic authentication
  scheme: basic
  type: http
slug: toshl-authentication
source_filename: toshl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.toshl.com/docs/\ndocs: https://developer.toshl.com/docs/oauth\ndescription: >\n  The Toshl API supports two authentication methods: OAuth 2.0 bearer tokens\n  (authorization code and implicit grants; user-revocable) and HTTP Basic\n  authentication using long-lived personal tokens created in the Toshl account\n  settings (apps section, available since 26 April 2016). Access tokens default\n  to a 3600-second lifetime with refresh tokens for renewal; refresh tokens can\n  be revoked by users or Toshl staff at any time. Client registration (client_id\n  and client_secret) is required before using OAuth.\nsummary:\n  types: [oauth2, http-basic]\n  oauth2_flows: [authorizationCode, implicit]\n  personal_tokens: true\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://toshl.com/oauth2/authorize\n        tokenUrl: https://toshl.com/oauth2/token\n\
  \        notes: Authorization code is valid for 30 seconds; token endpoint uses HTTP Basic auth with client credentials\n      - flow: implicit\n        authorizationUrl: https://toshl.com/oauth2/authorize\n        notes: For insecure clients; returns a token directly after user approval\n    token_lifetime_seconds: 3600\n    refresh_tokens: true\n    scopes_docs: https://developer.toshl.com/docs/oauth\n  - name: PersonalToken\n    type: http\n    scheme: basic\n    notes: Long-lived personal tokens generated in Toshl account settings, used via HTTP Basic authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toshl/refs/heads/main/authentication/toshl-authentication.yml
summary_line: oauth2/http-basic · 2 schemes
tags:
- Personal Finance
- Budgeting
- Expense Tracking
- FinTech
- Banking
- Consumer Apps
- Company
---
