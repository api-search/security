---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Overdrive Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: OverDrive secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: OverDrive
provider_slug: overdrive
scheme_count: 3
schemes:
- client_auth: basic
  client_auth_detail: 'Base64-encode "clientKey:clientSecret" (both case-sensitive) and send as Authorization: Basic {encoded}. POST with Content-Type: application/x-www-form-urlencoded;charset=UTF-8 and body grant_type=client_credentials.'
  flow: clientCredentials
  grant_type: client_credentials
  name: ClientAuthentication
  source: https://developer.overdrive.com/apis/client-auth
  token_ttl_seconds: 3600
  token_url: https://oauth.overdrive.com/token
  type: oauth2
  used_for:
  - Discovery APIs
  - Reporting APIs
  - Title Link API
- flow: clientCredentials
  grant_type: client_credentials
  name: PatronAuthentication
  notes: Exchanges library credentials for a patron collection token; OverDrive recommends using the resulting patron collection token for all subsequent calls once a user is authenticated.
  source: https://developer.overdrive.com/api-docs/authentication
  token_url: https://oauth-patron.overdrive.com/patrontoken
  type: oauth2
  used_for:
  - Circulation APIs
- name: QRCodeAuthentication
  notes: An alternative to credential-based patron authentication.
  source: https://developer.overdrive.com/api-docs/authentication
  type: oauth2
  used_for:
  - Circulation APIs
slug: overdrive-authentication
source_filename: overdrive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.overdrive.com/api-docs/authentication\ndocs: https://developer.overdrive.com/api-docs/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    OverDrive documents three authentication modes: client authentication\n    (OAuth 2.0 client-credentials, discovery-only), patron authentication\n    (adds a patron token for borrowing and holds), and QR-code authentication\n    (an alternative to credential-based patron sign-in). Access tokens are\n    valid for 3600 seconds and return the scopes granted to the credential.\nschemes:\n- name: ClientAuthentication\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://oauth.overdrive.com/token\n  grant_type: client_credentials\n  client_auth: basic\n  client_auth_detail: >-\n    Base64-encode \"clientKey:clientSecret\" (both case-sensitive) and send as\n    Authorization: Basic {encoded}. POST with\n    Content-Type:\
  \ application/x-www-form-urlencoded;charset=UTF-8 and\n    body grant_type=client_credentials.\n  token_ttl_seconds: 3600\n  used_for: [Discovery APIs, Reporting APIs, Title Link API]\n  source: https://developer.overdrive.com/apis/client-auth\n- name: PatronAuthentication\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://oauth-patron.overdrive.com/patrontoken\n  grant_type: client_credentials\n  used_for: [Circulation APIs]\n  notes: >-\n    Exchanges library credentials for a patron collection token; OverDrive\n    recommends using the resulting patron collection token for all subsequent\n    calls once a user is authenticated.\n  source: https://developer.overdrive.com/api-docs/authentication\n- name: QRCodeAuthentication\n  type: oauth2\n  used_for: [Circulation APIs]\n  notes: An alternative to credential-based patron authentication.\n  source: https://developer.overdrive.com/api-docs/authentication\nenvironments:\n  production:\n    discovery: https://api.overdrive.com/v1\n\
  \    circulation: https://patron.api.overdrive.com/v1\n    oauth: https://oauth.overdrive.com/token\n    patron_oauth: https://oauth-patron.overdrive.com/patrontoken\n  integration:\n    discovery: https://integration.api.overdrive.com\n    circulation: https://integration-patron.api.overdrive.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overdrive/refs/heads/main/authentication/overdrive-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Company
- Books
- Libraries
- Ebooks
- Audiobooks
- Digital Media
- Publishing
- Education
- Reading
- Circulation
---
