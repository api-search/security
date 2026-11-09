---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: microsoft-azure-communication-services-callautomation-api-openapi.yml
  format: yaml
  label: Azure Communication Services Call Automation API
  slug: microsoft-azure-communication-services-callautomation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-callautomation-api-openapi.yml
- filename: microsoft-azure-communication-services-chat-api-openapi.yml
  format: yaml
  label: Azure Communication Services Chat API
  slug: microsoft-azure-communication-services-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-chat-api-openapi.yml
- filename: microsoft-azure-communication-services-email-api-openapi.yml
  format: yaml
  label: Azure Communication Services Email API
  slug: microsoft-azure-communication-services-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-email-api-openapi.yml
- filename: microsoft-azure-communication-services-identity-api-openapi.yml
  format: yaml
  label: Azure Communication Services Identity API
  slug: microsoft-azure-communication-services-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-identity-api-openapi.yml
- filename: microsoft-azure-communication-services-jobrouter-api-openapi.yml
  format: yaml
  label: Azure Communication Services Job Router API
  slug: microsoft-azure-communication-services-jobrouter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml
- filename: microsoft-azure-communication-services-messages-api-openapi.yml
  format: yaml
  label: Azure Communication Services Advanced Messaging API
  slug: microsoft-azure-communication-services-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-messages-api-openapi.yml
- filename: microsoft-azure-communication-services-phonenumbers-api-openapi.yml
  format: yaml
  label: Azure Communication Services Phone Numbers API
  slug: microsoft-azure-communication-services-phonenumbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml
- filename: microsoft-azure-communication-services-rooms-api-openapi.yml
  format: yaml
  label: Azure Communication Services Rooms API
  slug: microsoft-azure-communication-services-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-rooms-api-openapi.yml
- filename: microsoft-azure-communication-services-siprouting-api-openapi.yml
  format: yaml
  label: Azure Communication Services SIP Routing API
  slug: microsoft-azure-communication-services-siprouting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml
- filename: microsoft-azure-communication-services-sms-api-openapi.yml
  format: yaml
  label: Azure Communication Services SMS API
  slug: microsoft-azure-communication-services-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-communication-services/openapi/microsoft-azure-communication-services-sms-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Microsoft Azure Communication Services Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Microsoft Azure Communication Services secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Microsoft Azure Communication Services
provider_slug: microsoft-azure-communication-services
scheme_count: 4
schemes:
- description: An Azure Communication Services user access token.
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/microsoft-azure-communication-services-callautomation-api-openapi.yml
  - openapi/microsoft-azure-communication-services-chat-api-openapi.yml
  - openapi/microsoft-azure-communication-services-email-api-openapi.yml
  - openapi/microsoft-azure-communication-services-messages-api-openapi.yml
  - openapi/microsoft-azure-communication-services-rooms-api-openapi.yml
  type: apiKey
- description: The Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: AadOauth2Auth
  sources:
  - openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml
  - openapi/microsoft-azure-communication-services-messages-api-openapi.yml
  type: oauth2
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml
  - openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml
  - openapi/microsoft-azure-communication-services-sms-api-openapi.yml
  type: oauth2
- description: An authentication string containing a signature generated using HMAC-SHA256 scheme.
  in: header
  name: apiKey
  parameter: access_key
  sources:
  - openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml
  type: apiKey
slug: microsoft-azure-communication-services-authentication
source_filename: microsoft-azure-communication-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-communication-services-callautomation-api-openapi.yml, openapi/microsoft-azure-communication-services-chat-api-openapi.yml,\n  openapi/microsoft-azure-communication-services-email-api-openapi.yml, openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml,\n  openapi/microsoft-azure-communication-services-messages-api-openapi.yml, openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml,\n  openapi/microsoft-azure-communication-services-rooms-api-openapi.yml, openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml,\n  openapi/microsoft-azure-communication-services-sms-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: An Azure Communication Services user access\
  \ token.\n  sources:\n  - openapi/microsoft-azure-communication-services-callautomation-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-chat-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-email-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-messages-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-rooms-api-openapi.yml\n- name: AadOauth2Auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n    scopes: 1\n  description: The Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/microsoft-azure-communication-services-jobrouter-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-messages-api-openapi.yml\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n\
  \    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n  sources:\n  - openapi/microsoft-azure-communication-services-phonenumbers-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml\n  - openapi/microsoft-azure-communication-services-sms-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: access_key\n  description: An authentication string containing a signature generated using HMAC-SHA256 scheme.\n  sources:\n  - openapi/microsoft-azure-communication-services-siprouting-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-communication-services/authentication/microsoft-azure-communication-services-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Microsoft Azure
- CPaaS
- Calling
- Chat
- Communications
- Contact Center
- Email
- Identity
- Messaging
- Phone Numbers
- Rooms
- Routing
- SIP
- SMS
- Telephony
- Tokens
- Video
- Voice
- WhatsApp
---
