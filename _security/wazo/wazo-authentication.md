---
api_key_in:
- header
api_specs:
- filename: wazo-auth-api-openapi.yml
  format: yaml
  label: Wazo Authentication API (wazo-auth)
  slug: wazo-authentication-api-wazo-auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-auth-api-openapi.yml
- filename: wazo-confd-api-openapi.yml
  format: yaml
  label: Wazo Configuration API (wazo-confd)
  slug: wazo-configuration-api-wazo-confd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-confd-api-openapi.yml
- filename: wazo-calld-api-openapi.yml
  format: yaml
  label: Wazo Call Control / Application API (wazo-calld)
  slug: wazo-call-control-application-api-wazo-calld
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-calld-api-openapi.yml
- filename: wazo-call-logd-api-openapi.yml
  format: yaml
  label: Wazo Call Detail Records API (wazo-call-logd)
  slug: wazo-call-detail-records-api-wazo-call-logd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-call-logd-api-openapi.yml
- filename: wazo-dird-api-openapi.yml
  format: yaml
  label: Wazo Directory & Contacts API (wazo-dird)
  slug: wazo-directory-contacts-api-wazo-dird
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-dird-api-openapi.yml
- filename: wazo-provd-api-openapi.yml
  format: yaml
  label: Wazo Phone Provisioning API (wazo-provd)
  slug: wazo-phone-provisioning-api-wazo-provd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-provd-api-openapi.yml
- filename: wazo-webhookd-api-openapi.yml
  format: yaml
  label: Wazo Webhooks API (wazo-webhookd)
  slug: wazo-webhooks-api-wazo-webhookd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-webhookd-api-openapi.yml
- filename: wazo-plugind-api-openapi.yml
  format: yaml
  label: Wazo Plugin Management API (wazo-plugind)
  slug: wazo-plugin-management-api-wazo-plugind
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-plugind-api-openapi.yml
- filename: wazo-agentd-api-openapi.yml
  format: yaml
  label: Wazo Call Centre Agent API (wazo-agentd)
  slug: wazo-call-centre-agent-api-wazo-agentd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-agentd-api-openapi.yml
- filename: wazo-chatd-api-openapi.yml
  format: yaml
  label: Wazo Presence & Chat API (wazo-chatd)
  slug: wazo-presence-chat-api-wazo-chatd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-chatd-api-openapi.yml
- filename: wazo-phoned-api-openapi.yml
  format: yaml
  label: Wazo Phone Directory & Service API (wazo-phoned)
  slug: wazo-phone-directory-service-api-wazo-phoned
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-phoned-api-openapi.yml
- filename: wazo-setupd-api-openapi.yml
  format: yaml
  label: Wazo Initial Setup API (wazo-setupd)
  slug: wazo-initial-setup-api-wazo-setupd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-setupd-api-openapi.yml
- filename: wazo-amid-api-openapi.yml
  format: yaml
  label: Wazo Asterisk Manager Interface API (wazo-amid)
  slug: wazo-asterisk-manager-interface-api-wazo-amid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-amid-api-openapi.yml
- filename: wazo-unattributed-asyncapi.yml
  format: yaml
  label: Wazo Websocket Event Stream (wazo-websocketd)
  slug: wazo-websocket-event-stream-wazo-websocketd
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/asyncapi/wazo-unattributed-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Wazo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wazo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wazo
provider_slug: wazo
scheme_count: 2
schemes:
- in: header
  name: wazo_auth_token
  parameter: X-Auth-Token
  sources:
  - openapi/wazo-agentd-api-openapi.yml
  - openapi/wazo-amid-api-openapi.yml
  - openapi/wazo-auth-api-openapi.yml
  - openapi/wazo-call-logd-api-openapi.yml
  - openapi/wazo-calld-api-openapi.yml
  - openapi/wazo-chatd-api-openapi.yml
  - openapi/wazo-confd-api-openapi.yml
  - openapi/wazo-dird-api-openapi.yml
  - openapi/wazo-phoned-api-openapi.yml
  - openapi/wazo-plugind-api-openapi.yml
  - openapi/wazo-provd-api-openapi.yml
  - openapi/wazo-setupd-api-openapi.yml
  - openapi/wazo-webhookd-api-openapi.yml
  type: apiKey
- name: wazo_auth_basic
  scheme: basic
  sources:
  - openapi/wazo-auth-api-openapi.yml
  type: http
slug: wazo-authentication
source_filename: wazo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/ (13 Swagger 2.0 contracts) + https://wazo-platform.org/uc-doc/api_sdk/rest_api/conventions + https://wazo-platform.org/uc-doc/api_sdk/rest_api/quickstart\n  + https://api.wazo.io/documentation/api/authentication.html\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: wazo_auth_token\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/wazo-agentd-api-openapi.yml\n  - openapi/wazo-amid-api-openapi.yml\n  - openapi/wazo-auth-api-openapi.yml\n  - openapi/wazo-call-logd-api-openapi.yml\n  - openapi/wazo-calld-api-openapi.yml\n  - openapi/wazo-chatd-api-openapi.yml\n  - openapi/wazo-confd-api-openapi.yml\n  - openapi/wazo-dird-api-openapi.yml\n  - openapi/wazo-phoned-api-openapi.yml\n  - openapi/wazo-plugind-api-openapi.yml\n  - openapi/wazo-provd-api-openapi.yml\n  - openapi/wazo-setupd-api-openapi.yml\n  - openapi/wazo-webhookd-api-openapi.yml\n- name:\
  \ wazo_auth_basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/wazo-auth-api-openapi.yml\ndocs: https://api.wazo.io/documentation/overview/authentication.html\nmodel:\n  style: opaque bearer token in a custom header, issued by a first-party token service\n  header: X-Auth-Token\n  oauth2: false\n  oidc: false\n  token_endpoint: POST https://{wazo_stack}/api/auth/0.1/token\n  token_endpoint_auth: HTTP Basic username:password (the wazo_auth_basic scheme), or an existing refresh token\n  recommended_user_purpose: external_api\n  token_expiration: requested per token via the expiration field (seconds); tokens expire and must be renewed\n  introspection:\n  - HEAD /token/{token} — validity\n  - GET /token/{token} — metadata incl. ACL list\n  - POST /token/{token}/scopes/check — pre-flight an ACL\n  revocation: DELETE /token/{token}\n  refresh_tokens: GET /tokens lists refresh tokens created for the caller\n  warning: The quickstart states that a manually generated token \"gives all\
  \ permissions to anyone who knows it\" — Wazo ships\n    no default least-privilege token. Scoping requires creating an ACL policy (POST /policies) and attaching it.\nauthorization:\n  model: acl\n  catalog: scopes/wazo-acl-permissions.yml\n  permission_count: 788\n  declaration: each operation states \"**Required ACL:** `<string>`\" in its own description\n  wildcards:\n    one_segment: '*'\n    remainder: '#'\n  multi_tenancy:\n    header: Wazo-Tenant\n    recurse_param: recurse\nidentity_backends:\n  first_party:\n  - wazo_user (username/password)\n  federated:\n  - LDAP — POST/GET /backends/ldap\n  - SAML 2.0 — /saml/sso, /saml/acs, /saml/logout, /saml/sls, /backends/saml, /backends/saml/metadata\n  external_auth:\n  - Google\n  - Microsoft\n  - mobile push (FCM/APNs registration)\n  source: openapi/wazo-auth-api-openapi.yml\nmutual_tls: false\napi_keys: false\napi_keys_note: There is no long-lived API key. Programmatic access means minting a short-lived token from user credentials,\n\
  \  or holding a refresh token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/authentication/wazo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Telephony
- VoIP
- Unified Communications
- UCaaS
- Contact Center
- SIP
- asterisk
- WebRTC
- Open-Source
- Self-Hosted
- White Label
- PBX
- MSP
- Call Center
- Provisioning
- Webhook
- Event-Driven
- Chat
- Presence
- CDR
---
