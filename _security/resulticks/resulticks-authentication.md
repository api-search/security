---
api_key_in:
- unknown
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Resulticks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Resulticks secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Resulticks
provider_slug: resulticks
scheme_count: 2
schemes:
- credentials_endpoint: https://apis.resu.io/Apirsltks/Credentials
  credentials_method: GET
  credentials_parameters:
  - name: Username
    type: string
  - name: Password
    type: string
  description: An API key is issued by a credentials endpoint rather than a console. The documented call is GET https://apis.resu.io/Apirsltks/Credentials with Username (string) and Password (string) parameters; a 200 response returns an `apiKey` (string) and a 401 returns Unauthorized. The docs do not state which header or query parameter the returned key is subsequently presented in, nor a key TTL/rotation policy.
  in: unknown
  name: ResulApiKey
  parameter_name: unknown
  responses:
  - returns: apiKey (string)
    status: 200
  - returns: Unauthorized
    status: 401
  sources:
  - https://gud.resulticks.com/API-reference/API-management/API-keys/
  type: apiKey
- authorization_url: null
  description: The API gateway page states "the third-party systems utilize the OAuth protocol for authenticating REST API calls." No authorization URL, token URL, grant type, or scope list is published anywhere in the public documentation, so the flow cannot be modelled.
  flows: []
  name: OAuth2
  scopes_published: false
  sources:
  - https://gud.resulticks.com/API-reference/API-management/API-gateway/
  token_url: null
  type: oauth2
slug: resulticks-authentication
source_filename: resulticks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://gud.resulticks.com/API-reference/API-management/API-keys/\ndocs: https://gud.resulticks.com/API-reference/API-management/API-keys/\nnote: >-\n  Derived from the Resulticks (RESUL) public documentation portal at\n  gud.resulticks.com. Resulticks publishes no OpenAPI/Swagger definition, so no\n  securitySchemes could be read mechanically; this profile is transcribed from\n  the provider's own API-management reference pages.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - unknown\n  oauth2_flows: []\n  spec_backed: false\nschemes:\n- name: ResulApiKey\n  type: apiKey\n  description: >-\n    An API key is issued by a credentials endpoint rather than a console. The\n    documented call is GET https://apis.resu.io/Apirsltks/Credentials with\n    Username (string) and Password (string) parameters; a 200 response returns\n    an `apiKey` (string) and a 401 returns Unauthorized. The docs do not state\n    which\
  \ header or query parameter the returned key is subsequently presented\n    in, nor a key TTL/rotation policy.\n  credentials_endpoint: https://apis.resu.io/Apirsltks/Credentials\n  credentials_method: GET\n  credentials_parameters:\n  - name: Username\n    type: string\n  - name: Password\n    type: string\n  responses:\n  - status: 200\n    returns: apiKey (string)\n  - status: 401\n    returns: Unauthorized\n  in: unknown\n  parameter_name: unknown\n  sources:\n  - https://gud.resulticks.com/API-reference/API-management/API-keys/\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The API gateway page states \"the third-party systems utilize the OAuth\n    protocol for authenticating REST API calls.\" No authorization URL, token\n    URL, grant type, or scope list is published anywhere in the public\n    documentation, so the flow cannot be modelled.\n  flows: []\n  authorization_url: null\n  token_url: null\n  scopes_published: false\n  sources:\n  - https://gud.resulticks.com/API-reference/API-management/API-gateway/\n\
  authorization:\n  model: role-and-permission\n  description: >-\n    The API reference exposes Manage role and Manage permission pages,\n    indicating account-level RBAC over Resul objects rather than OAuth scopes.\n    The \"API Keys\" call category is documented as being \"for management of\n    accounts and permissions on Resul objects.\"\n  docs:\n  - https://gud.resulticks.com/API-reference/manage-role/\n  - https://gud.resulticks.com/API-reference/manage-permission/\ngaps:\n- No OAuth authorization/token endpoint, grant type, or scope reference is published.\n- The header or parameter carrying the issued apiKey on subsequent calls is not documented.\n- No key rotation, expiry, or revocation policy is published.\n- >-\n  The base host apis.resu.io resolves in DNS (35.227.61.169) but refused TCP on\n  both 443 and 80 from the public internet on 2026-08-13, so no live\n  authentication behaviour could be observed.\nx-evidence:\n- url: https://gud.resulticks.com/API-reference/API-management/API-keys/\n\
  \  status: 200\n- url: https://gud.resulticks.com/API-reference/API-management/API-gateway/\n  status: 200\n- url: https://gud.resulticks.com/API-reference/API-management/web-API-controllers/\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resulticks/refs/heads/main/authentication/resulticks-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Marketing
- Marketing Automation
- Omnichannel
- Customer Engagement
- Customer Data Platform
- MarTech
- Campaign Management
- Audience
- Analytics
- Messaging
- SMS
- Email
- Push Notifications
- WhatsApp
---
