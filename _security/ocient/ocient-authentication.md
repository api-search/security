---
api_key_in: []
api_specs:
- filename: ocient-ocient-http-query-api-api-openapi.yml
  format: yaml
  label: Ocient Ocient HTTP Query API API
  slug: ocient-ocient-http-query-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocient/refs/heads/main/openapi/ocient-ocient-http-query-api-api-openapi.yml
- filename: ocient-system-information-rest-endpoints-api-openapi.yml
  format: yaml
  label: Ocient System Information REST Endpoints API
  slug: ocient-system-information-rest-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocient/refs/heads/main/openapi/ocient-system-information-rest-endpoints-api-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ocient Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
- authorizationCode
- tokenExchange
overview: Ocient secures its APIs with http and openIdConnect across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode, authorizationCode, and tokenExchange flow(s).
provider_name: Ocient
provider_slug: ocient
scheme_count: 0
schemes: []
slug: ocient-authentication
source_filename: ocient-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.ocient.com/authentication-methods\ndocs: https://docs.ocient.com/authentication-methods\nrelated_docs:\n- https://docs.ocient.com/ocient-http-query-api\n- https://docs.ocient.com/ocient-security-guide\n- https://docs.ocient.com/database-password-security-settings\n- https://docs.ocient.com/manage-users-groups-and-roles\nsummary:\n  types: [http, openIdConnect]\n  http_schemes: [basic, bearer]\n  api_key_in: []\n  oauth2_flows: [deviceCode, authorizationCode, tokenExchange]\n  spec_declares_security_schemes: false\n  spec_note: 'The published OpenAPI declares an empty components.securitySchemes and\n    `security: []`. Authentication is modelled instead as a required `authorization`\n    / `Authorization` header parameter on the protected operations. The auth model\n    below is taken from the documentation, not inferred from the spec.'\nmethods:\n- id: password\n  name: Password authentication\n  type: http\n \
  \ schemes: [basic, bearer]\n  description: Users created with DCL set a password used for database authentication.\n    Callers may present HTTP Basic credentials directly, or exchange them at the login\n    endpoint for a bearer token.\n  username_format: '<user_name>@<database>'\n  username_format_name: Fully Qualified User Name (FQUN)\n  username_example: alice@example_database\n  operations:\n    login: postOcientHttpQueryApiLogin\n    logout: postOcientHttpQueryApiLogout\n    refresh: postOcientHttpQueryApiTokenRefresh\n  policy_controls: https://docs.ocient.com/database-password-security-settings\n  policy_notes: Administrators can configure minimum password length and password\n    expiration policies.\n- id: sso-oidc\n  name: OpenID Connect single sign-on\n  type: openIdConnect\n  description: Administrators can add a Single Sign-On integration so users authenticate\n    against an external OpenID Connect identity provider. A database, including the\n    system database, can have\
  \ 0 or 1 SSO integrations. The presence of an SSO\n    integration has no effect on users authenticating with a password.\n  identity_providers: any OIDC provider (Okta documented as example)\n  flows:\n  - id: authorizationCode\n    description: Browser redirect flow — initiate at sso_authentication, the\n      authorization server redirects to the callback path which yields the token.\n    operations: [postOcientHttpQueryApiSsoAuthentication, getOcientHttpQueryApiCallback]\n  - id: deviceCode\n    description: Device grant flow for headless clients — retrieve a device grant\n      code, have the user approve it, then verify to receive an authorization token.\n    operations: [postOcientHttpQueryApiSsoDeviceGrant, postOcientHttpQueryApiSsoDeviceGrantVerify]\n  - id: tokenExchange\n    description: Exchange an OpenID Connect identifier token or access token for an\n      Ocient access token.\n    operations: [postOcientHttpQueryApiSsoToken]\n  mfa: Ocient recommends multi-factor authentication\
  \ for all accounts accessing an\n    Ocient System, and limiting local accounts to emergency SSO-recovery access.\ntoken_handling:\n  transport: Authorization header, Bearer scheme\n  session_cookie: The login operation also sets a session cookie.\n  refresh:\n    operation: postOcientHttpQueryApiTokenRefresh\n    guidance: Call before the current token expires to maintain uninterrupted access.\n  revocation:\n    logout_invalidates_tokens: false\n    note: Logout clears associated cookies but does not invalidate access tokens.\nauthorization:\n  model: role-based access control\n  docs: https://docs.ocient.com/manage-users-groups-and-roles\n  features:\n  - Default System and Database Roles\n  - Administrator-defined access groups scoped to tables, rows, or views\n  - Object-type level privileges management\n  guidance: Ocient recommends assigning roles on least privilege, separation of duties,\n    and need-to-know.\ntransport_security:\n  tls: The SQL service always has TLS functionality\
  \ enabled and active.\n  docs: https://docs.ocient.com/secure-connections-using-tls\n  note: By default the database allows both encrypted and unencrypted JDBC connections\n    even when server certificates are present; enforcing TLS-only is a deployment\n    hardening step.\ndriver_authentication:\n  jdbc: 'connect to jdbc:ocient://<host>:<port>/<database>;user=<fqun>;password=****;'\n  pyocient: Same FQUN and password model via the Python DB-API 2.0 driver.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocient/refs/heads/main/authentication/ocient-authentication.yml
summary_line: http/openIdConnect · 0 schemes
tags:
- Company
- Data
- Analytics
- Data Warehouse
- Database
- SQL
- Artificial Intelligence
- Machine-Learning
- Big Data
- Geospatial
---
