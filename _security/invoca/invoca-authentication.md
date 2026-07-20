---
api_key_in:
- header
- body
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Invoca Authentication
name_suffix: Authentication
oauth_flows: []
overview: Invoca secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Invoca
provider_slug: invoca
scheme_count: 3
schemes:
- description: Recommended. Send the self-serve Invoca API token in the Authorization request header. Tokens are long-lived (no refresh token) and must be treated like passwords; never commit to source control.
  format: 'Authorization: <token>'
  in: header
  name: InvocaAPIToken
  parameter: Authorization
  sources:
  - https://developers.invoca.net/en/latest/api_documentation/manage_api_credentials.html
  type: apiKey
- description: 'Alternative for JSON POST requests: pass the token as an oauth_token key/value pair in the JSON request body.'
  in: body
  name: InvocaAPITokenBody
  parameter: oauth_token
  sources:
  - https://developers.invoca.net/en/latest/api_documentation/manage_api_credentials.html
  type: apiKey
- description: HTTP(S) Basic Authentication using a username and password in the request header. Supported alongside API tokens on the transactions/network surface.
  name: HTTPBasic
  scheme: basic
  sources:
  - https://developers.invoca.net/en/latest/basics/design_principles.html
  type: http
slug: invoca-authentication
source_filename: invoca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.invoca.net/en/latest/api_documentation/manage_api_credentials.html\ndocs: https://developers.invoca.net/en/latest/basics/design_principles.html\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - body\n  notes: >-\n    Invoca's self-serve API access is token-based and OAuth-compliant, but does\n    NOT use OAuth refresh tokens and exposes no OAuth scope surface. Tokens are\n    minted per-credential in the platform UI (Integrations > Manage Integrations\n    > Invoca APIs > + New API Credential). HTTP(S) Basic Authentication (username\n    + password) is also accepted, and session-login auth is available for browser\n    testing only.\nschemes:\n- name: InvocaAPIToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: <token>'\n  description: >-\n    Recommended. Send the self-serve Invoca API token in the Authorization\n    request header. Tokens are\
  \ long-lived (no refresh token) and must be treated\n    like passwords; never commit to source control.\n  sources:\n  - https://developers.invoca.net/en/latest/api_documentation/manage_api_credentials.html\n- name: InvocaAPITokenBody\n  type: apiKey\n  in: body\n  parameter: oauth_token\n  description: >-\n    Alternative for JSON POST requests: pass the token as an oauth_token\n    key/value pair in the JSON request body.\n  sources:\n  - https://developers.invoca.net/en/latest/api_documentation/manage_api_credentials.html\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  description: >-\n    HTTP(S) Basic Authentication using a username and password in the request\n    header. Supported alongside API tokens on the transactions/network surface.\n  sources:\n  - https://developers.invoca.net/en/latest/basics/design_principles.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invoca/refs/heads/main/authentication/invoca-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Ai
- Call Tracking
- Conversation Intelligence
- Marketing
- Attribution
- Revenue
- Telephony
- Analytics
---
