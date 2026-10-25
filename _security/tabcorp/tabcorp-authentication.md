---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tabcorp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tabcorp secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tabcorp
provider_slug: tabcorp
scheme_count: 1
schemes:
- authorizationUrl: https://api.beta.tab.com.au/oauth/authorize
  description: 'Applicants are issued a client_id and client_secret; the Digital API uses OAuth 2.0 and credentials are exchanged for a short-lived Bearer token sent as ''Authorization: Bearer <token>''. Token responses show expires_in: 10800 and token_type: bearer.'
  flows:
    authorization_code: Delegated authorisation (3-legged OAuth) for applications acting on behalf of any TAB customer; customer is redirected to tab.com.au; client_id must be configured for this access.
    client_credentials: Informational use only, for applications that only need non-customer data e.g. racing feeds, odds and results.
    password: Single customer API access; requires TAB account number and password (or account_pin) plus brand=TAB; API support must enable password grant for the account.
    refresh_token: Post API credentials with refresh_token to receive a new access_token with the same scopes.
  grant_types:
  - client_credentials
  - password
  - authorization_code
  - refresh_token
  name: TAB Digital API OAuth 2.0
  scheme: bearer
  sources:
  - https://web.archive.org/web/20170219083237/https://studio.tab.com.au/intro/authentication.html
  - https://web.archive.org/web/20170219083239/https://studio.tab.com.au/intro/authentication/client-credentials-grant.html
  - https://web.archive.org/web/20170219083241/https://studio.tab.com.au/intro/authentication/password-grant.html
  - https://web.archive.org/web/20170219083244/https://studio.tab.com.au/intro/authentication/auth-code-grant.html
  - https://web.archive.org/web/20170219083250/https://studio.tab.com.au/intro/authentication/refresh-tokens.html
  tokenUrl: https://api.beta.tab.com.au/oauth/token
  type: oauth2
slug: tabcorp-authentication
source_filename: tabcorp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://web.archive.org/web/20170219083237/https://studio.tab.com.au/intro/authentication.html\ndocs: https://studio.tab.com.au/intro/authentication.html\nnote: \"Live TAB Studio docs (www.studio.tab.com.au) answered 403 Akamai Access Denied (geo-restricted) on 2026-10-22; content read from the Internet Archive snapshot of the provider's own docs, captured February 2017, and may be out of date.\"\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: TAB Digital API OAuth 2.0\n  type: oauth2\n  scheme: bearer\n  description: \"Applicants are issued a client_id and client_secret; the Digital API uses OAuth 2.0 and credentials are exchanged for a short-lived Bearer token sent as 'Authorization: Bearer <token>'. Token responses show expires_in: 10800 and token_type: bearer.\"\n  tokenUrl: https://api.beta.tab.com.au/oauth/token\n  authorizationUrl: https://api.beta.tab.com.au/oauth/authorize\n  grant_types:\n  - client_credentials\n\
  \  - password\n  - authorization_code\n  - refresh_token\n  flows:\n    client_credentials: \"Informational use only, for applications that only need non-customer data e.g. racing feeds, odds and results.\"\n    password: \"Single customer API access; requires TAB account number and password (or account_pin) plus brand=TAB; API support must enable password grant for the account.\"\n    authorization_code: \"Delegated authorisation (3-legged OAuth) for applications acting on behalf of any TAB customer; customer is redirected to tab.com.au; client_id must be configured for this access.\"\n    refresh_token: \"Post API credentials with refresh_token to receive a new access_token with the same scopes.\"\n  sources:\n  - https://web.archive.org/web/20170219083237/https://studio.tab.com.au/intro/authentication.html\n  - https://web.archive.org/web/20170219083239/https://studio.tab.com.au/intro/authentication/client-credentials-grant.html\n  - https://web.archive.org/web/20170219083241/https://studio.tab.com.au/intro/authentication/password-grant.html\n\
  \  - https://web.archive.org/web/20170219083244/https://studio.tab.com.au/intro/authentication/auth-code-grant.html\n  - https://web.archive.org/web/20170219083250/https://studio.tab.com.au/intro/authentication/refresh-tokens.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabcorp/refs/heads/main/authentication/tabcorp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Wagering
- Betting
- Gaming
- Media
- Racing
- Australia
---
