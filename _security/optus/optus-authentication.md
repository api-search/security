---
api_key_in:
- header
api_specs:
- filename: optus-delete-multiple-lists-api-openapi.yml
  format: yaml
  label: Optus Delete Multiple Lists API
  slug: optus-delete-multiple-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-delete-multiple-lists-api-openapi.yml
- filename: optus-documentation-api-openapi.yml
  format: yaml
  label: Optus Documentation API
  slug: optus-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-documentation-api-openapi.yml
- filename: optus-lists-api-openapi.yml
  format: yaml
  label: Optus Lists API
  slug: optus-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-lists-api-openapi.yml
- filename: optus-messages-api-openapi.yml
  format: yaml
  label: Optus Messages API
  slug: optus-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-messages-api-openapi.yml
- filename: optus-report-api-openapi.yml
  format: yaml
  label: Optus Report API
  slug: optus-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-report-api-openapi.yml
- filename: optus-scheduled-campaigns-api-openapi.yml
  format: yaml
  label: Optus Scheduled Campaigns API
  slug: optus-scheduled-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-scheduled-campaigns-api-openapi.yml
- filename: optus-services-api-openapi.yml
  format: yaml
  label: Optus Services API
  slug: optus-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-services-api-openapi.yml
- filename: optus-status-api-openapi.yml
  format: yaml
  label: Optus Status API
  slug: optus-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-status-api-openapi.yml
- filename: optus-templates-api-openapi.yml
  format: yaml
  label: Optus Templates API
  slug: optus-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-templates-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Optus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Optus secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Optus
provider_slug: optus
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/optus-sms-suite-campaign-manager-openapi.yml
  - openapi/optus-sms-suite-rest-v1-openapi.yml
  type: http
- description: HTTP Basic Authentication is used for all authenticated requests.
  in: header
  name: GatewayAuthorizer
  note: Modelled in the spec as an apiKey in the Authorization header, but the value is a standard HTTP Basic credential. Functionally identical to BasicAuth.
  parameter: Authorization
  sources:
  - openapi/optus-sms-suite-rest-v2-openapi.yml
  type: apiKey
slug: optus-authentication
source_filename: optus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  openapi/optus-sms-suite-campaign-manager-openapi.yml, openapi/optus-sms-suite-rest-v1-openapi.yml,\n  openapi/optus-sms-suite-rest-v2-openapi.yml\ndocs: https://sms.optus.com.au/docs/en/security/\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  model: http-basic-only\n  oauth2: false\n  oidc: false\n  mtls: false\n  ciba: false\n  note: >-\n    Every authenticated Optus SMS Suite interface uses HTTP Basic with per-application\n    credentials. There is no OAuth 2.0, no OpenID Connect, no bearer token, no scope model, no\n    mutual TLS, and no key-issuance API. /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server return 404 on every Optus host.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/optus-sms-suite-campaign-manager-openapi.yml\n  - openapi/optus-sms-suite-rest-v1-openapi.yml\n- name: GatewayAuthorizer\n  type: apiKey\n \
  \ in: header\n  parameter: Authorization\n  description: HTTP Basic Authentication is used for all authenticated requests.\n  sources:\n  - openapi/optus-sms-suite-rest-v2-openapi.yml\n  note: >-\n    Modelled in the spec as an apiKey in the Authorization header, but the value is a standard\n    HTTP Basic credential. Functionally identical to BasicAuth.\ncredential_issuance:\n  self_service: false\n  where: >-\n    Generated inside the platform, per application, at\n    https://sms.optus.com.au/gateway/api_config/{rest|restv2|http|soap|smpp|mms}. Requires a\n    platform login.\n  username: the application name\n  password: platform-generated per application\n  rotation: not documented\n  api: none - there is no API to create, list, rotate, or revoke credentials\nby_interface:\n- {api: SMS Gateway REST API v1, mechanism: HTTP Basic (Authorization header), spec: openapi/optus-sms-suite-rest-v1-openapi.yml}\n- {api: SMS Gateway REST API v2, mechanism: HTTP Basic via the GatewayAuthorizer\
  \ scheme, spec: openapi/optus-sms-suite-rest-v2-openapi.yml}\n- {api: Campaign Manager API, mechanism: HTTP Basic, per-operation security, spec: openapi/optus-sms-suite-campaign-manager-openapi.yml}\n- {api: 2FA REST API, mechanism: HTTP Basic, spec: null, media_type: application/vnd.modica.2fa.v1+json}\n- {api: REST Email API, mechanism: HTTP Basic, spec: null}\n- {api: MM7 MMS API, mechanism: HTTP Basic, spec: null}\n- {api: SOAP API, mechanism: application name + password in the SOAP request, contract: 'https://api.sms.optus.com.au/ModicaSoap.wsdl'}\n- {api: HTTPS API, mechanism: 'application and password as query-string parameters', spec: null, note: 'credentials travel in the URL - unavoidable on this legacy interface, and one reason it is deprecation-announced'}\n- {api: SMPP API, mechanism: 'system_id + password on bind, max 8 characters, over mandatory TLS 1.2+ on port 2776', spec: null}\n- {api: Health Monitoring API, mechanism: none, spec: openapi/optus-sms-suite-status-openapi.json,\
  \ note: deliberately unauthenticated}\n- {api: Callbacks (DLR/MO), mechanism: 'optional Basic credentials embedded in the configured callback URL (must be URL-encoded)', note: subscriber-side}\n- {api: MM7 callbacks, mechanism: HTTP Basic required, note: 'the provider requires Basic auth on all MM7 callback URLs'}\nnetwork_controls:\n  ip_allowlisting:\n    supported: true\n    scope: per application\n    behaviour: >-\n      Optional and default-off. Once one or more IPs or ranges are registered under \"Authorised\n      IP Addresses\", every other source IP is rejected with an authentication error.\n  tls_minimum: TLS 1.2\n  https_enforced: true\nplatform_identity:\n  note: >-\n    Distinct from API authentication - these govern human access to the SMS Suite web platform,\n    not API calls.\n  federated_id:\n    supported: true\n    protocol: SAML 2.0\n    docs: https://sms.optus.com.au/docs/en/security/federated-identity/\n  scim:\n    supported: true\n    version: '2.0'\n    docs:\
  \ https://sms.optus.com.au/docs/en/security/scim/\n  mfa: supported\ngaps:\n- No OAuth 2.0 or OpenID Connect anywhere on the public surface.\n- No scopes, so authorisation is all-or-nothing per application credential.\n- No credential lifecycle API (create/rotate/revoke) and no documented rotation policy.\n- No CIBA, which CAMARA specifies alongside OIDC for network-based authorization.\n- Credentials on the legacy HTTPS API travel in the query string.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/authentication/optus-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Telecommunications
- Australia
- Mobile Network Operator
- Messaging
- SMS
- MMS
- Two-Factor Authentication
- Network APIs
- CAMARA
- Open Gateway
- IoT
- 5G
- Broadband
- Satellite
- Enterprise
---
