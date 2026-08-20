---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mirrorfly Messages Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: MirrorFly Messages API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MirrorFly Messages API
provider_slug: mirrorfly-messages-api
scheme_count: 1
schemes:
- format: 'Opaque token sent as the raw value of the Authorization header (documented as `-H "Authorization: AuthToken"`). The docs show no "Bearer " prefix.'
  in: header
  name: AuthToken
  parameter_name: Authorization
  scheme: custom-token
  sources:
  - https://www.mirrorfly.com/docs/platformapi/adminapis/get-started/
  token_lifetime: 3600
  token_lifetime_note: '"Authentication token received in the response is valid upto 1 hour. You need to call the API once again to generate the new token." A 401 on a secured API is the documented signal to re-mint.'
  type: http
slug: mirrorfly-messages-api-authentication
source_filename: mirrorfly-messages-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: >-\n  https://www.mirrorfly.com/docs/platformapi/userapis/getstarted/login/ and\n  https://www.mirrorfly.com/docs/platformapi/adminapis/get-started/\ndocs: https://www.mirrorfly.com/docs/platformapi/userapis/getstarted/login/\nnote: >-\n  Derived by reading the published docs, not from an OpenAPI — MirrorFly publishes no\n  machine-readable specification. There are two separate credential sets (User API and\n  Admin API), each minting its own token from the same login operation shape.\nsummary:\n  types: [http]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: AuthToken\n    type: http\n    scheme: custom-token\n    in: header\n    parameter_name: Authorization\n    format: >-\n      Opaque token sent as the raw value of the Authorization header (documented as\n      `-H \"Authorization: AuthToken\"`). The docs show no \"Bearer \" prefix.\n    token_lifetime:\
  \ 3600\n    token_lifetime_note: >-\n      \"Authentication token received in the response is valid upto 1 hour. You need to\n      call the API once again to generate the new token.\" A 401 on a secured API is the\n      documented signal to re-mint.\n    sources: [https://www.mirrorfly.com/docs/platformapi/adminapis/get-started/]\ntoken_endpoint:\n  method: POST\n  path: /api/v1/login\n  url_template: https://{api-base-url}/api/v1/login\n  content_type: application/json\n  request:\n    - {name: username, type: string, required: true, description: Username provided by the admin/console}\n    - {name: password, type: string, required: true, description: Password provided by the admin/console}\n  response_shape: '{ \"status\": 200, \"data\": { \"token\": \"...\" }, \"message\": \"Data retrieved successfully\" }'\n  error_shape: '{ \"status\": 400, \"message\": \"Error Message\" }'\naudiences:\n  - name: User API\n    credentials: username + password for an end user\n    docs: https://www.mirrorfly.com/docs/platformapi/userapis/getstarted/login/\n\
  \  - name: Admin API\n    credentials: admin username + password from the MirrorFly console\n    docs: https://www.mirrorfly.com/docs/platformapi/adminapis/get-started/\ncredential_issuance:\n  console: https://console.mirrorfly.com/\n  registration: https://www.mirrorfly.com/contact-sales.php\n  gate: >-\n    Credentials are not self-service. The docs route \"Register here\" to the contact-sales\n    form and state \"Registration is subject to verification and would take up to 24 hours.\"\n    For Eazy plan and paid subscribers, API credentials appear in the console only after\n    the customer supplies their server configuration.\n  base_url: >-\n    Production {api-base-url} is tenant-specific and issued through the console; the\n    public preprod sandbox host is api-preprod-sandbox.mirrorfly.com.\nobservations:\n  - No OAuth 2.0, OpenID Connect, mTLS or scoped-permission model is documented.\n  - No API-key rotation, key-prefix, or key-scoping documentation was found.\n  - No /.well-known/openid-configuration\
  \ or /.well-known/oauth-authorization-server is served.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirrorfly-messages-api/refs/heads/main/authentication/mirrorfly-messages-api-authentication.yml
summary_line: http · 1 scheme
tags:
- CPaaS
- Communications
- Chat / Messaging API
- Voice API
- Video API
- SIP/VoIP
- Real-Time Communication
- SDK
- Self-hosted / On-premise
- AI Agents / Chatbots
- Contact Center
---
