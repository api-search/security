---
api_key_in: []
api_specs:
- filename: kurly-kls-fulfillment-openapi.yml
  format: yaml
  label: Kurly Logistics Services (KLS) Fulfillment API
  slug: kurly-logistics-services-kls-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-kls-fulfillment-openapi.yml
- filename: kurly-kls-delivery-agency-openapi.yml
  format: yaml
  label: Kurly Logistics Services (KLS) Delivery Agency API
  slug: kurly-logistics-services-kls-delivery-agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-kls-delivery-agency-openapi.yml
- filename: kurly-kls-delivery-tracking-openapi.yml
  format: yaml
  label: Kurly Logistics Services (KLS) Delivery Tracking API
  slug: kurly-logistics-services-kls-delivery-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-kls-delivery-tracking-openapi.yml
- filename: kurly-kls-auth-openapi.yml
  format: yaml
  label: Kurly Logistics Services (KLS) Authentication API
  slug: kurly-logistics-services-kls-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-kls-auth-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kurly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kurly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kurly
provider_slug: kurly
scheme_count: 1
schemes:
- description: 'Access token issued by POST /auth/token using the clientId/secretKey pair Kurly issues after IP allowlist registration. Sent as `Authorization: Bearer {AccessToken}`.'
  docs: https://developers.kurly.com/docs/auth
  format: Bearer {AccessToken}
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kurly-kls-delivery-agency-openapi.yml
  - openapi/kurly-kls-delivery-tracking-openapi.yml
  - openapi/kurly-kls-fulfillment-openapi.yml
  type: http
slug: kurly-authentication
source_filename: kurly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.kurly.com/docs/auth\ndocs: https://developers.kurly.com/docs/auth\napi: Kurly Logistics Services (KLS) Open API\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  self_service: false\n  network_control: ip-allowlist\n\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Access token issued by POST /auth/token using the clientId/secretKey pair Kurly issues after IP\n    allowlist registration. Sent as `Authorization: Bearer {AccessToken}`.\n  header: Authorization\n  format: 'Bearer {AccessToken}'\n  sources:\n  - openapi/kurly-kls-delivery-agency-openapi.yml\n  - openapi/kurly-kls-delivery-tracking-openapi.yml\n  - openapi/kurly-kls-fulfillment-openapi.yml\n  docs: https://developers.kurly.com/docs/auth\n\ntoken_issuance:\n  operation: issueToken\n  endpoint: POST\
  \ /auth/token\n  credentials:\n  - clientId\n  - secretKey\n  docs: https://developers.kurly.com/docs/api/인증/토큰-발급\n  responses:\n    '200': Authentication succeeded (인증 성공)\n    '400': Authentication error (인증 오류)\n  expiry: not published\n  refresh: not published\n\ncredential_issuance:\n  self_service: false\n  process: >-\n    The shipper submits the list of IP addresses that will call the API via Kurly's Google Form.\n    Kurly issues the clientId and secretKey by reply within a maximum of 5 business days.\n  form: https://docs.google.com/forms/d/18MuePJjYaalk6KOXF61Mts6hVPJAyDlxndK_Q8SjxBs/edit\n  turnaround: up to 5 business days\n  prerequisite: an existing fulfillment or delivery-agency contract with Kurly\n  docs: https://developers.kurly.com/docs/auth\n\nnetwork_controls:\n  ip_allowlist:\n    required: true\n    description: >-\n      Calls are only accepted from IPs the shipper registered with Kurly. Allowlisting is a\n      precondition of credential issuance, not an optional\
  \ hardening step.\n    docs: https://developers.kurly.com/docs/intro\n\nscopes:\n  supported: false\n  note: >-\n    KLS has no OAuth scope or permission surface — authorisation is implied by the shipper's contract\n    and the credentials issued against it. No scopes/ artifact is emitted for this provider.\n\ntest_environment:\n  available: true\n  self_service: false\n  requirements:\n  - Complete Kurly security training (보안 교육 수료)\n  - Sign a security pledge (보안 서약서 작성)\n  - Follow the VPN and firewall guidance\n  artifact: sandbox/kurly-sandbox.yml\n  docs: https://developers.kurly.com/docs/faq\n\nsupport:\n  email: logistics-dev@kurlycorp.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/authentication/kurly-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Technology
- Logistics
- Fulfillment
- Supply Chain
- Delivery
- Ecommerce
- Grocery
- Shipping
- Order Management
- Inventory
- Tracking
- South Korea
---
