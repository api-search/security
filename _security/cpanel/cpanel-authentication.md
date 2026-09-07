---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cpanel-uapi-openapi.yml
  format: yaml
  label: cPanel UAPI
  slug: uapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/openapi/cpanel-uapi-openapi.yml
- filename: cpanel-whm-api-openapi.yml
  format: yaml
  label: WHM API 1
  slug: whm-api-1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/openapi/cpanel-whm-api-openapi.yml
auth_types:
- http
- api-key-in-authorization-header
description: 'cPanel & WHM authentication. The OpenAPI documents are thin here — both declare exactly one `BasicAuth` http scheme and nothing else — so the token forms below come from the developer documentation, which is where cPanel actually specifies them. Note the two custom `Authorization` prefixes: they are NOT `Bearer`, and a client that sends `Bearer` will fail.'
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Cpanel Authentication
name_suffix: Authentication
oauth_flows: []
overview: cPanel secures its APIs with http and api-key-in-authorization-header across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: cPanel
provider_slug: cpanel
scheme_count: 6
schemes:
- caution: cPanel's own guidance prefers secure remote logins over username/password in code. Two-factor authentication does not apply to username/password API calls by default, though it can be enforced in WHM's Configure Security Policies interface.
  description: HTTP Basic authentication with a cPanel account username and password (UAPI, ports 2082/2083 and Webmail 2095/2096) or a WHM/reseller username and password (WHM API 1, ports 2086/2087).
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/_original/cpanel-uapi-openapi.yml
  - openapi/_original/cpanel-whm-api-openapi.yml
  spec_declared: true
  type: http
- applies_to:
  - cPanel UAPI
  - cPanel API 2
  description: A cPanel-account API token. Created in cPanel's Manage API Tokens interface or via UAPI Tokens-create_full_access; usable outside a browser session on ports 2082/2083.
  docs: https://api.docs.cpanel.net/cpanel/tokens/
  example_call: 'curl -H''Authorization: cpanel username:APITOKEN'' ''https://example.com:2083/execute/Email/add_pop?email=newuser&password=...'''
  format: 'Authorization: cpanel <username>:<APITOKEN>'
  header: Authorization
  in: header
  name: cPanelApiToken
  scheme_prefix: 'cpanel '
  spec_declared: false
  type: apiKey
- applies_to:
  - WHM API 1
  - cPanel UAPI via WHM API 1
  description: A WHM API token for the root user or a reseller. Created in WHM's Manage API Tokens interface or via WHM API 1 Tokens-api_token_create; revoked via Tokens-api_token_revoke. Ports 2087, or 443 through a service subdomain.
  docs: https://api.docs.cpanel.net/whm/tokens/
  format: 'Authorization: whm <username>:<token>'
  header: Authorization
  in: header
  lifecycle_caution: cPanel documents that an expired API token is NOT removed automatically — it must be deleted by hand.
  name: WhmApiToken
  scheme_prefix: 'whm '
  spec_declared: false
  type: apiKey
- description: 'Access hashes authenticate as the root user. cPanel documents them alongside API tokens but the WHM API 1 operations that expose them — Resellers-accesshash and Resellers-get_remote_access_hash — are marked deprecated: true in the contract.'
  docs: https://api.docs.cpanel.net/guides/guide-to-api-authentication/guide-to-api-authentication-access-hash-authentication/
  header: Authorization
  in: header
  name: AccessHash
  spec_declared: false
  status: legacy
  type: apiKey
- description: Browser/cookie-based calls made from inside a cPanel, Webmail or WHM session must carry the session's security token in the URL path (the `cpsess##########` segment). This is the in-product path, not an integration path.
  docs: https://api.docs.cpanel.net/guides/guide-to-api-authentication/guide-to-api-authentication-browser-based-authentication/
  name: SessionSecurityToken
  spec_declared: false
  type: session
- description: Generates a temporary session to authenticate with cPanel & WHM.
  docs: https://api.docs.cpanel.net/guides/guide-to-api-authentication/guide-to-api-authentication-single-sign-on/
  name: SingleSignOn
  spec_declared: false
  type: sso
slug: cpanel-authentication
source_filename: cpanel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  openapi/_original/cpanel-uapi-openapi.yml + openapi/_original/cpanel-whm-api-openapi.yml\n  (securitySchemes), upgraded from https://api.docs.cpanel.net/guides/guide-to-api-authentication/,\n  https://api.docs.cpanel.net/cpanel/tokens/ and https://api.docs.cpanel.net/whm/tokens/\ndocs: https://api.docs.cpanel.net/guides/guide-to-api-authentication/\nprovider: cPanel\nproviderId: cpanel\ndescription: >-\n  cPanel & WHM authentication. The OpenAPI documents are thin here — both declare exactly one\n  `BasicAuth` http scheme and nothing else — so the token forms below come from the developer\n  documentation, which is where cPanel actually specifies them. Note the two custom\n  `Authorization` prefixes: they are NOT `Bearer`, and a client that sends `Bearer` will fail.\nsummary:\n  types: [http, api-key-in-authorization-header]\n  spec_declared: [BasicAuth]\n  documented_additional: [cPanel API token, WHM API token, access\
  \ hash, session security token, SSO]\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    spec_declared: true\n    description: >-\n      HTTP Basic authentication with a cPanel account username and password (UAPI, ports\n      2082/2083 and Webmail 2095/2096) or a WHM/reseller username and password (WHM API 1,\n      ports 2086/2087).\n    sources: [openapi/_original/cpanel-uapi-openapi.yml, openapi/_original/cpanel-whm-api-openapi.yml]\n    caution: >-\n      cPanel's own guidance prefers secure remote logins over username/password in code. Two-factor\n      authentication does not apply to username/password API calls by default, though it can be\n      enforced in WHM's Configure Security Policies interface.\n  - name: cPanelApiToken\n    type: apiKey\n    in: header\n    header: Authorization\n    scheme_prefix: 'cpanel '\n    format: 'Authorization: cpanel <username>:<APITOKEN>'\n    spec_declared: false\n    applies_to: [cPanel UAPI, cPanel API 2]\n    description:\
  \ >-\n      A cPanel-account API token. Created in cPanel's Manage API Tokens interface or via UAPI\n      Tokens-create_full_access; usable outside a browser session on ports 2082/2083.\n    docs: https://api.docs.cpanel.net/cpanel/tokens/\n    example_call: >-\n      curl -H'Authorization: cpanel username:APITOKEN'\n      'https://example.com:2083/execute/Email/add_pop?email=newuser&password=...'\n  - name: WhmApiToken\n    type: apiKey\n    in: header\n    header: Authorization\n    scheme_prefix: 'whm '\n    format: 'Authorization: whm <username>:<token>'\n    spec_declared: false\n    applies_to: [WHM API 1, cPanel UAPI via WHM API 1]\n    description: >-\n      A WHM API token for the root user or a reseller. Created in WHM's Manage API Tokens\n      interface or via WHM API 1 Tokens-api_token_create; revoked via Tokens-api_token_revoke.\n      Ports 2087, or 443 through a service subdomain.\n    docs: https://api.docs.cpanel.net/whm/tokens/\n    lifecycle_caution: >-\n      cPanel\
  \ documents that an expired API token is NOT removed automatically — it must be\n      deleted by hand.\n  - name: AccessHash\n    type: apiKey\n    in: header\n    header: Authorization\n    spec_declared: false\n    status: legacy\n    description: >-\n      Access hashes authenticate as the root user. cPanel documents them alongside API tokens\n      but the WHM API 1 operations that expose them — Resellers-accesshash and\n      Resellers-get_remote_access_hash — are marked deprecated: true in the contract.\n    docs: https://api.docs.cpanel.net/guides/guide-to-api-authentication/guide-to-api-authentication-access-hash-authentication/\n  - name: SessionSecurityToken\n    type: session\n    spec_declared: false\n    description: >-\n      Browser/cookie-based calls made from inside a cPanel, Webmail or WHM session must carry the\n      session's security token in the URL path (the `cpsess##########` segment). This is the\n      in-product path, not an integration path.\n    docs: https://api.docs.cpanel.net/guides/guide-to-api-authentication/guide-to-api-authentication-browser-based-authentication/\n\
  \  - name: SingleSignOn\n    type: sso\n    spec_declared: false\n    description: Generates a temporary session to authenticate with cPanel & WHM.\n    docs: https://api.docs.cpanel.net/guides/guide-to-api-authentication/guide-to-api-authentication-single-sign-on/\noauth:\n  rest_apis: false\n  agent_surfaces: true\n  note: >-\n    No OAuth anywhere on the REST surface. OAuth appears only on the two MCP endpoints — see\n    scopes/cpanel-scopes.yml.\nports:\n  - port: 2082\n    surface: cPanel UAPI / cPanel API 2\n    tls: false\n  - port: 2083\n    surface: cPanel UAPI / cPanel API 2\n    tls: true\n  - port: 2086\n    surface: WHM API 1\n    tls: false\n  - port: 2087\n    surface: WHM API 1\n    tls: true\n  - port: 2095\n    surface: cPanel UAPI via Webmail session\n    tls: false\n  - port: 2096\n    surface: cPanel UAPI via Webmail session\n    tls: true\nports_note: >-\n  cPanel documents that an otherwise-correct call on the wrong port returns \"Permission denied\"\n  or \"Function\
  \ not found\" — an authentication failure that reads like a routing failure.\nauthorization:\n  model: privileges-and-roles\n  notes:\n    - API tokens carry privileges; a full-access cPanel token is created by Tokens-create_full_access.\n    - Reseller privileges bound WHM API 1 access below root.\n    - >-\n      Server profiles (roles) DISABLE whole modules: the contract repeats \"When you disable the\n      [role], the system disables this function\" across many operations, so a 200-with-error can\n      mean the role is off rather than the credential being wrong.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/authentication/cpanel-authentication.yml
summary_line: http/api-key-in-authorization-header · 6 schemes
tags:
- Control Panel
- DNS
- Domains
- Email
- Hosting
- Reseller
- Server Administration
- Web Hosting
- WHM
---
