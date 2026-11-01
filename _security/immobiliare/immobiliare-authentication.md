---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Immobiliare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Immobiliare.it declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Immobiliare.it
provider_slug: immobiliare
scheme_count: 1
schemes:
- client_authentication: HTTP Basic with <clientID>:<secretkey>
  flow: password
  grant_type: password (username and password of the customer account)
  name: oauth2-password
  refresh_token: returned in the example response (refresh_token field); the docs do not describe a refresh flow
  request_content_type: application/x-www-form-urlencoded
  token_endpoint: POST {base_url}/oauth/token
  token_lifetime: Your access token remains valid for 4 hours; once it expires, request a new one.
  token_type: Bearer
  type: oauth2
  usage: 'Authorization: Bearer <token>'
slug: immobiliare-authentication
source_filename: immobiliare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://insights.immobiliare.it/webdocs/authentication/\ndocs: https://insights.immobiliare.it/webdocs/authentication/\nschemes:\n- name: oauth2-password\n  type: oauth2\n  flow: password\n  token_endpoint: POST {base_url}/oauth/token\n  client_authentication: HTTP Basic with <clientID>:<secretkey>\n  request_content_type: application/x-www-form-urlencoded\n  grant_type: password (username and password of the customer account)\n  token_type: Bearer\n  token_lifetime: Your access token remains valid for 4 hours; once it expires, request a new one.\n  refresh_token: returned in the example response (refresh_token field); the docs do not describe a refresh flow\n  usage: 'Authorization: Bearer <token>'\nnotes:\n- 'Every service getting-started page states: \"All the requests do require an OAUTH 2.0 auth token in the header,\n  see the authentication page for details.\"'\n- 'Docs warn: \"excessive authentication traffic can be\
  \ flagged by our protection systems and may lead to a temporary\n  ban.\" Store and reuse the token.'\n- Credentials are issued to customers; no self-serve signup is documented. The token endpoint was read from the\n  docs, never called.\n"
source_yaml_url: https://artifacts.apis.io/immobiliare/authentication/immobiliare-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Real Estate
- Property Listings
- Italy
- Marketplaces
- Open Source
---
