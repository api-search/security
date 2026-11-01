---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods supported by SlashDB as documented.
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Slashdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: VT Enterprise declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: VT Enterprise
provider_slug: slashdb
scheme_count: 5
schemes:
- evidence: HTTP Basic Authentication
  header: Authorization
  location: header
  name: HTTP Basic Authentication
  type: http-basic
- authorize_url: authorization_endpoint
  evidence: OpenID Connect is an authentication layer on top of the OAuth 2.0 authorization framework.
  header: Authorization
  how_to_obtain: Obtain client_id and configure redirect_uri, then follow the OpenID Connect flow using the IdP.
  location: header
  name: OpenID Connect (JWT)
  scopes:
  - openid
  - email
  token_url: token_endpoint
  type: http-bearer
- evidence: API Key
  name: API Key
  type: apiKey
- evidence: Cookie Session
  name: Cookie Session
  type: other
- evidence: Public (unauthenticated) access
  name: Public Access
  type: other
slug: slashdb-authentication
source_filename: slashdb-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.slashdb.com/user-guide/security/authentication/
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.slashdb.com/user-guide/security/authentication/\nsources:\n- https://docs.slashdb.com/user-guide/security/authentication/\n- https://docs.slashdb.com/user-guide/config/db_credentials/\n- https://docs.slashdb.com/user-guide/security/encrypting-credentials/\ndescription: Authentication methods supported by SlashDB as documented.\nschemes:\n- type: http-basic\n  name: HTTP Basic Authentication\n  evidence: HTTP Basic Authentication\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: OpenID Connect (JWT)\n  evidence: OpenID Connect is an authentication layer on top of the OAuth 2.0 authorization framework.\n  location: header\n  header: Authorization\n  token_url: token_endpoint\n  authorize_url: authorization_endpoint\n  scopes:\n  - openid\n  - email\n  how_to_obtain: Obtain client_id and configure redirect_uri, then follow the OpenID Connect flow\
  \ using the IdP.\n- type: apiKey\n  name: API Key\n  evidence: API Key\n- type: other\n  name: Cookie Session\n  evidence: Cookie Session\n- type: other\n  name: Public Access\n  evidence: Public (unauthenticated) access\ndocs: https://docs.slashdb.com/user-guide/security/authentication/\n"
source_yaml_url: https://artifacts.apis.io/slashdb/authentication/slashdb-authentication.yml
summary_line: 5 schemes
tags:
- API
- Data Integration
- Low Code
- Enterprise Software
- Database APIs
---
