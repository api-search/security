---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: E6Data Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: e6data secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: e6data
provider_slug: e6data
scheme_count: 4
schemes:
- docs: https://docs.e6data.com/product-documentation/user-settings/personal-access-tokens-pat
  format: Bearer <ACCESS_TOKEN>
  header: Authorization
  location: header
  name: PersonalAccessToken
  notes: Recommended method. Tokens are created in the console (User Settings > Access Token) with an optional expiry in days and are shown only once. Used as the Bearer token for the REST Query Count API and as the JDBC password (with the cluster username). A cluster restart is required each time a new PAT is created for JDBC use.
  scheme: bearer
  type: http
- docs: https://docs.e6data.com/product-documentation/access-control/service-accounts
  location: header
  name: ServiceAccount
  notes: Non-user programmatic identity assigned an RBAC role; generates a downloadable key file (typically CSV). Up to 10 keys per service account. RBAC role changes take effect immediately for all API requests.
  scheme: bearer
  type: http
- docs: https://docs.e6data.com/product-documentation/access-control/single-sign-on-sso
  flow: authorizationCode
  name: SSO
  notes: Console sign-in only (human users), not API authorization. No API-level OAuth scope surface is published; programmatic access is governed by RBAC roles/permissions/policies rather than OAuth scopes.
  providers:
  - AWS SSO / IAM Identity Center
  - Okta
  - AWS Cognito (OAuth 2.0)
  - Microsoft Entra ID
  - Google IdP
  type: oauth2
- docs: https://docs.e6data.com/product-documentation/access-control/multi-factor-authentication-beta
  name: MFA
  notes: Additional verification layer for console login (beta).
  status: beta
  type: mfa
slug: e6data-authentication
source_filename: e6data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.e6data.com/product-documentation/access-control\ndocs: https://docs.e6data.com/product-documentation/user-settings/personal-access-tokens-pat\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Programmatic access to e6data (Python connector, JDBC driver, REST Query\n    Count API, BI tools) authenticates with a Personal Access Token (PAT)\n    presented as a Bearer token, or a username + PAT pair for JDBC. Service\n    Accounts provide non-user programmatic credentials (downloadable key file,\n    max 10 keys) scoped by RBAC role. Console/user login is federated via SSO\n    (SAML/OAuth 2.0) and optional MFA.\nschemes:\n  - name: PersonalAccessToken\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: \"Bearer <ACCESS_TOKEN>\"\n    docs: https://docs.e6data.com/product-documentation/user-settings/personal-access-tokens-pat\n\
  \    notes: >-\n      Recommended method. Tokens are created in the console (User Settings >\n      Access Token) with an optional expiry in days and are shown only once.\n      Used as the Bearer token for the REST Query Count API and as the JDBC\n      password (with the cluster username). A cluster restart is required each\n      time a new PAT is created for JDBC use.\n  - name: ServiceAccount\n    type: http\n    scheme: bearer\n    location: header\n    docs: https://docs.e6data.com/product-documentation/access-control/service-accounts\n    notes: >-\n      Non-user programmatic identity assigned an RBAC role; generates a\n      downloadable key file (typically CSV). Up to 10 keys per service account.\n      RBAC role changes take effect immediately for all API requests.\n  - name: SSO\n    type: oauth2\n    flow: authorizationCode\n    docs: https://docs.e6data.com/product-documentation/access-control/single-sign-on-sso\n    providers:\n      - AWS SSO / IAM Identity Center\n  \
  \    - Okta\n      - AWS Cognito (OAuth 2.0)\n      - Microsoft Entra ID\n      - Google IdP\n    notes: >-\n      Console sign-in only (human users), not API authorization. No API-level\n      OAuth scope surface is published; programmatic access is governed by RBAC\n      roles/permissions/policies rather than OAuth scopes.\n  - name: MFA\n    type: mfa\n    status: beta\n    docs: https://docs.e6data.com/product-documentation/access-control/multi-factor-authentication-beta\n    notes: Additional verification layer for console login (beta).\nauthorization:\n  model: RBAC\n  docs: https://docs.e6data.com/product-documentation/access-control\n  primitives: [users, groups, roles, permissions, policies]\n  data_level: row-level and column-level access controls (column masking, row filtering)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/e6data/refs/heads/main/authentication/e6data-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Company
- B2B
- Data
- Analytics
- Lakehouse
- SQL
- Query Engine
- Data Infrastructure
- Big Data
---
