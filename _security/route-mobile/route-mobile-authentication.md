---
api_key_in:
- header
- query
- body
api_specs:
- filename: route-mobile-sms.yml
  format: yaml
  label: Route Mobile SMS API
  slug: route-mobile-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-sms.yml
- filename: route-mobile-whatsapp-business.yml
  format: yaml
  label: Route Mobile WhatsApp Business API
  slug: route-mobile-whatsapp-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-whatsapp-business.yml
- filename: route-mobile-rcs.yml
  format: yaml
  label: Route Mobile RCS Business Messaging API
  slug: route-mobile-rcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-rcs.yml
- filename: route-mobile-viber.yml
  format: yaml
  label: Route Mobile Viber Business Messages API
  slug: route-mobile-viber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-viber.yml
- filename: route-mobile-sendclean-email.yml
  format: yaml
  label: SendClean Email API
  slug: sendclean-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-sendclean-email.yml
- filename: Enterprise-Voice-2.0-APIs
  format: yaml
  label: Route Mobile Enterprise Voice 2.0 API
  slug: route-mobile-enterprise-voice-api
  spec_type: Postman
  url: https://github.com/routemobile/Enterprise-Voice-2.0-APIs
auth_types:
- apiKey
- http
- query-credentials
- body-credentials
description: 'Route Mobile''s authentication is legacy CPaaS rather than telco-standard, and it is not uniform: four different credential models across five products. There is no OAuth 2.0, no OpenID Connect, no discovery document (/.well-known/openid-configuration and /.well-known/oauth-authorization-server 404 on every host), and no scopes — so no scopes/ artifact is emitted for this provider. Two of the models (SMS query-parameter credentials, SendClean body-carried token) are not expressible as OpenAPI securitySchemes and are therefore absent from the specs; they were harvested from the documentation and from the operation parameters.'
kind: authentication
layout: security
method: searched
name: Route Mobile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Route Mobile secures its APIs with apiKey, http, query-credentials, and body-credentials across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Route Mobile
provider_slug: route-mobile
scheme_count: 5
schemes:
- description: JWT minted by POST /auth/v1/login/ on apis.rmlconnect.net and carried in the Authorization header. Declared as an apiKey-in-header scheme in the RCS and Viber definitions.
  in: header
  name: jwt
  parameter: Authorization
  sources:
  - openapi/route-mobile-rcs.yml
  - openapi/route-mobile-viber.yml
  type: apiKey
- bearerFormat: JWT
  description: JSON Web Token obtained from the WhatsApp Login API (POST /auth/v1/login/). Include the token in the `Authorization` header as `Bearer <token>`. Tokens expire after one hour by default.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/route-mobile-whatsapp-business.yml
  type: http
- description: Static authorization token issued by Route Mobile, used only by the MoEngage and WebEngage integration endpoints on the SMS API.
  in: header
  name: AuthorizationToken
  parameter: Authorization
  sources:
  - openapi/route-mobile-sms.yml
  type: apiKey
- description: The core SMS API authenticates with the account username and password passed as URL query parameters on every GET request over HTTPS. Not expressible as an OpenAPI securityScheme; documented on the SMS reference pages and present as required parameters on every operation. A separate GET /bulksms/generatetoken mints a short-lived token consumed by GET /bulksms/bulksubmit.
  in: query
  name: sms-query-credentials
  parameters:
  - username
  - password
  sources:
  - openapi/route-mobile-sms.yml
  - https://developer.rmlconnect.net/route-mobile-project/reference/sendsmssecured
  type: query-credentials
- description: SendClean carries `owner_id` and `token` inside the JSON request body of every POST (and as URL-encoded query parameters on the single HTTP GET operation). No Authorization header is used. Declared in the spec as the reusable AuthFields schema rather than as a securityScheme.
  in: body
  name: sendclean-body-credentials
  parameters:
  - owner_id
  - token
  sources:
  - openapi/route-mobile-sendclean-email.yml
  type: body-credentials
slug: route-mobile-authentication
source_filename: route-mobile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/route-mobile-rcs.yml, openapi/route-mobile-sms.yml, openapi/route-mobile-viber.yml,\n  openapi/route-mobile-whatsapp-business.yml, openapi/route-mobile-sendclean-email.yml\ndocs:\n- https://developer.rmlconnect.net/route-mobile-project/docs/whatsapp-login\n- https://developer.rmlconnect.net/route-mobile-project/reference/sendsmssecured\n- https://developer.rmlconnect.net/route-mobile-project/docs/email\ndescription: >-\n  Route Mobile's authentication is legacy CPaaS rather than telco-standard, and it is not\n  uniform: four different credential models across five products. There is no OAuth 2.0, no\n  OpenID Connect, no discovery document (/.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server 404 on every host), and no scopes — so no scopes/\n  artifact is emitted for this provider. Two of the models (SMS query-parameter credentials,\n  SendClean body-carried token) are not expressible as\
  \ OpenAPI securitySchemes and are\n  therefore absent from the specs; they were harvested from the documentation and from the\n  operation parameters.\nsummary:\n  types: [apiKey, http, query-credentials, body-credentials]\n  api_key_in: [header, query, body]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  scopes: false\n  uniform_across_products: false\nschemes:\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    JWT minted by POST /auth/v1/login/ on apis.rmlconnect.net and carried in the Authorization\n    header. Declared as an apiKey-in-header scheme in the RCS and Viber definitions.\n  sources:\n  - openapi/route-mobile-rcs.yml\n  - openapi/route-mobile-viber.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    JSON Web Token obtained from the WhatsApp Login API (POST /auth/v1/login/). Include the\n    token in the `Authorization` header as `Bearer <token>`. Tokens\
  \ expire after one hour by\n    default.\n  sources:\n  - openapi/route-mobile-whatsapp-business.yml\n- name: AuthorizationToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Static authorization token issued by Route Mobile, used only by the MoEngage and WebEngage\n    integration endpoints on the SMS API.\n  sources:\n  - openapi/route-mobile-sms.yml\n- name: sms-query-credentials\n  type: query-credentials\n  in: query\n  parameters: [username, password]\n  description: >-\n    The core SMS API authenticates with the account username and password passed as URL query\n    parameters on every GET request over HTTPS. Not expressible as an OpenAPI securityScheme;\n    documented on the SMS reference pages and present as required parameters on every\n    operation. A separate GET /bulksms/generatetoken mints a short-lived token consumed by\n    GET /bulksms/bulksubmit.\n  sources:\n  - openapi/route-mobile-sms.yml\n  - https://developer.rmlconnect.net/route-mobile-project/reference/sendsmssecured\n\
  - name: sendclean-body-credentials\n  type: body-credentials\n  in: body\n  parameters: [owner_id, token]\n  description: >-\n    SendClean carries `owner_id` and `token` inside the JSON request body of every POST (and\n    as URL-encoded query parameters on the single HTTP GET operation). No Authorization header\n    is used. Declared in the spec as the reusable AuthFields schema rather than as a\n    securityScheme.\n  sources:\n  - openapi/route-mobile-sendclean-email.yml\ntoken_lifecycle:\n  whatsapp: JWT expires after one hour by default; re-login on 401.\n  rcs_viber: JWT from POST /auth/v1/login/; expiry not documented.\n  sms: >-\n    Username/password are long-lived account credentials; the optional generatetoken token is\n    short-lived and single-purpose.\n  sendclean: Long-lived account token; no documented rotation endpoint.\ntransport_security:\n  https_required: true\n  legacy_plaintext: >-\n    The SMS definition still lists http://api.rmlconnect.net as an \"SGN Non-secured\
  \ (HTTP) —\n    legacy only\" server. Sending account credentials as query parameters over that host would\n    expose them in cleartext; use the HTTPS servers (port 443 or 8443) only.\ngaps:\n- No OAuth 2.0 / OpenID Connect anywhere, hence no scopes and no consent surface.\n- Credentials in URLs (SMS) leak into proxy, gateway and browser-history logs.\n- No mutual TLS, no signed requests, and no key-rotation endpoint outside SendClean's webhook key.\nrelated:\n  conventions: conventions/route-mobile-conventions.yml\n  domain_security: security/route-mobile-domain-security.yml\n  conformance: conformance/route-mobile-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/authentication/route-mobile-authentication.yml
summary_line: apiKey/http/query-credentials/body-credentials · 5 schemes
tags:
- Telecommunications
- India
- CPaaS
- Messaging
- SMS
- A2P Messaging
- WhatsApp Business
- RCS
- Voice
- Email
- Identity Verification
- OTP
- Aggregator
---
