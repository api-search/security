---
api_key_in: []
auth_types:
- oauth2
- password-login
description: ''
kind: authentication
layout: security
method: probed
name: Odaseva Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Odaseva secures its APIs with oauth2 and password-login across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Odaseva
provider_slug: odaseva
scheme_count: 2
schemes:
- authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
  dpop: true
  id_token_signing_alg_values_supported:
  - RS256
  introspectionUrl: https://login.salesforce.com/services/oauth2/introspect
  issuer: https://login.salesforce.com
  jwksUri: https://login.salesforce.com/id/keys
  name: SalesforcePlatformOIDC
  note: 'OWNERSHIP: this discovery document is Salesforce''s, served from Odaseva''s Salesforce My Domain hosts. It describes the Salesforce platform authorization server, and its scopes (api, full, refresh_token, offline_access, cdp_*, mcp_api, ...) are Salesforce platform scopes — NOT Odaseva-defined scopes. It is recorded because it is the real, observable way the Odaseva platform host authenticates callers, and it is the reason no scopes/ artifact is written: Odaseva publishes no scope vocabulary of its own.'
  openIdConnectUrl: https://api.odaseva.com/.well-known/openid-configuration
  owner: salesforce
  revocationUrl: https://login.salesforce.com/services/oauth2/revoke
  sources:
  - well-known/odaseva-api-openid-configuration.json
  tokenUrl: https://login.salesforce.com/services/oauth2/token
  type: openIdConnect
  userinfoUrl: https://login.salesforce.com/services/oauth2/userinfo
- credentials:
  - Odaseva username
  - Odaseva password
  - Odaseva Org Id
  - Odaseva endpoint alias
  name: OdasevaCliLogin
  note: 'Strings read verbatim out of the published odaseva-cli binary: "Odaseva username", "Odaseva password", "Access token", "Odaseva Org Id", "Odaseva endpoint alias", "User successfully logged in.", "Session expired!", "The password is expired. Login failed." No API-key mechanism appears anywhere in the published surface.'
  owner: odaseva
  scheme: password-then-bearer-token
  sources:
  - packages/odaseva-packages.yml
  - cli/odaseva-cli.yml
  token: access token (stored in ~/.odaseva_cli; "Session expired!" on expiry)
  type: http
slug: odaseva-authentication
source_filename: odaseva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: >-\n  Live probes of api.odaseva.com and platform.odaseva.com plus the first-party\n  odaseva-cli@2022.12.0 npm release; no OpenAPI exists to derive from\n  (derive-authentication.py found 0 auth profiles for this provider).\npointer_note: >-\n  DELIBERATELY NOT WIRED as a `type: Authentication` pointer in apis.yml. Odaseva publishes\n  NO public authentication documentation — this file is our probe record, not a provider\n  document, and emitting the pointer would credit Odaseva with a documented auth surface it\n  does not publish. Re-evaluate if Odaseva ever puts an auth page or spec on a public URL.\nsummary:\n  types:\n  - oauth2\n  - password-login\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  identity_provider: Salesforce (login.salesforce.com)\n  public_docs: false\nhosts:\n- host: api.odaseva.com\n  role: Odaseva Platform API host (Salesforce My Domain, Visualforce /CBR/ namespace)\n\
  \  unauthenticated_response: 401 on every probed API and .well-known path except OIDC discovery\n  ip_space: Salesforce (155.226.157.0/24)\n- host: platform.odaseva.com\n  role: Odaseva Console / platform login (https://platform.odaseva.com/CBR, HTTP 200)\n  unauthenticated_response: 301 at root, 401 on API paths\nschemes:\n- name: SalesforcePlatformOIDC\n  type: openIdConnect\n  owner: salesforce\n  openIdConnectUrl: https://api.odaseva.com/.well-known/openid-configuration\n  issuer: https://login.salesforce.com\n  authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n  tokenUrl: https://login.salesforce.com/services/oauth2/token\n  revocationUrl: https://login.salesforce.com/services/oauth2/revoke\n  introspectionUrl: https://login.salesforce.com/services/oauth2/introspect\n  userinfoUrl: https://login.salesforce.com/services/oauth2/userinfo\n  jwksUri: https://login.salesforce.com/id/keys\n  id_token_signing_alg_values_supported:\n  - RS256\n  dpop: true\n  sources:\n\
  \  - well-known/odaseva-api-openid-configuration.json\n  note: >-\n    OWNERSHIP: this discovery document is Salesforce's, served from Odaseva's Salesforce My\n    Domain hosts. It describes the Salesforce platform authorization server, and its\n    scopes (api, full, refresh_token, offline_access, cdp_*, mcp_api, ...) are Salesforce\n    platform scopes — NOT Odaseva-defined scopes. It is recorded because it is the real,\n    observable way the Odaseva platform host authenticates callers, and it is the reason\n    no scopes/ artifact is written: Odaseva publishes no scope vocabulary of its own.\n- name: OdasevaCliLogin\n  type: http\n  scheme: password-then-bearer-token\n  owner: odaseva\n  credentials:\n  - Odaseva username\n  - Odaseva password\n  - Odaseva Org Id\n  - Odaseva endpoint alias\n  token: access token (stored in ~/.odaseva_cli; \"Session expired!\" on expiry)\n  sources:\n  - packages/odaseva-packages.yml\n  - cli/odaseva-cli.yml\n  note: >-\n    Strings read verbatim out\
  \ of the published odaseva-cli binary: \"Odaseva username\",\n    \"Odaseva password\", \"Access token\", \"Odaseva Org Id\", \"Odaseva endpoint alias\",\n    \"User successfully logged in.\", \"Session expired!\", \"The password is expired. Login\n    failed.\" No API-key mechanism appears anywhere in the published surface.\nevidence:\n- url: https://api.odaseva.com/.well-known/openid-configuration\n  status: 200\n- url: https://api.odaseva.com/openapi.json\n  status: 401\n- url: https://platform.odaseva.com/.well-known/openid-configuration\n  status: 200\n- url: https://platform.odaseva.com/CBR\n  status: 200\ngaps:\n- No public authentication documentation page.\n- No published OpenAPI securitySchemes (no spec at all).\n- No Odaseva-defined OAuth scopes; the visible scope set belongs to the Salesforce platform.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odaseva/refs/heads/main/authentication/odaseva-authentication.yml
summary_line: oauth2/password-login · 2 schemes
tags:
- Company
- Infrastructure Saas
- Salesforce
- Data Protection
- Backup
- Data Governance
- Security
- Compliance
- Privacy
---
