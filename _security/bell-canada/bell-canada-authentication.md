---
api_key_in:
- header
api_specs:
- filename: bell-canada-trouble-ticket-api-openapi.json
  format: json
  label: Bell Canada Trouble Ticket API
  slug: bell-canada-trouble-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-trouble-ticket-api-openapi.json
- filename: bell-canada-service-order-api-openapi.json
  format: json
  label: Bell Canada Service Order API
  slug: bell-canada-service-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-service-order-api-openapi.json
- filename: bell-canada-resource-inventory-api-openapi.json
  format: json
  label: Bell Canada Resource Inventory Management API
  slug: bell-canada-resource-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-resource-inventory-api-openapi.json
- filename: bell-canada-change-management-api-openapi.json
  format: json
  label: Bell Canada Change Management API
  slug: bell-canada-change-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-change-management-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bell Canada Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bell Canada secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bell Canada
provider_slug: bell-canada
scheme_count: 2
schemes:
- declared_in_spec: false
  evidence: Every documented curl / Python / PHP / Java example on the four API reference pages redacts the credential as a literal header placeholder --header 'SECURITY_CREDENTIALS'. The real header name and value are supplied to an approved partner by email; Bell does not publish them.
  in: header
  name: SECURITY_CREDENTIALS
  parameter: SECURITY_CREDENTIALS
  source: https://developer.bell.ca/troubleticket
  status: placeholder-published
  type: apiKey
- declared_in_spec: false
  evidence: Documented on every example request as "for use in sandbox mode only, pass any unique value >= 8 chars". A sandbox caller-identity header, not a secret.
  in: header
  name: x-external-system
  parameter: x-external-system
  scope: sandbox-only
  source: https://developer.bell.ca/troubleticket
  type: apiKey
slug: bell-canada-authentication
source_filename: bell-canada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/*.json (no securityDefinitions) + https://developer.bell.ca/faq/apis\ndocs: https://developer.bell.ca/faq/apis\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  spec_declared: false\n  issuance: out-of-band\n  self_serve: false\n  note: >-\n    None of the four harvested Swagger 2.0 documents declares a securityDefinitions block or a\n    security requirement, so the credential model is documented only in prose on the developer\n    portal. Bell issues API keys manually after a business registration is reviewed and approved\n    by a Bell administrator; the user ID, the API endpoint and the credentials arrive by email.\n    There is no self-serve key issuance, no OAuth 2.0, no OpenID Connect discovery document and\n    no published authorization or token URL.\nschemes:\n- name: SECURITY_CREDENTIALS\n  type: apiKey\n  in: header\n  parameter: SECURITY_CREDENTIALS\n  declared_in_spec: false\n\
  \  source: https://developer.bell.ca/troubleticket\n  evidence: >-\n    Every documented curl / Python / PHP / Java example on the four API reference pages redacts the\n    credential as a literal header placeholder --header 'SECURITY_CREDENTIALS'. The real header\n    name and value are supplied to an approved partner by email; Bell does not publish them.\n  status: placeholder-published\n- name: x-external-system\n  type: apiKey\n  in: header\n  parameter: x-external-system\n  declared_in_spec: false\n  source: https://developer.bell.ca/troubleticket\n  evidence: >-\n    Documented on every example request as \"for use in sandbox mode only, pass any unique value\n    >= 8 chars\". A sandbox caller-identity header, not a secret.\n  scope: sandbox-only\nissuance:\n  process: >-\n    Register on https://developer.bell.ca/register with business details. \"After registration,\n    requests will be assessed and validated by a Bell administrator. The Bell administrator will\n    get in touch\
  \ with the requestor and send a user ID, API end point and other details via email\n    after verification. Using these credentials and API end point, the API can now be accessed.\"\n  source: https://developer.bell.ca/faq/apis\n  self_serve: false\n  approval: manual\n  credential_delivery: email\ntransport_security:\n  tls_minimum: TLSv1.2\n  cipher_note: 256 bit SHA2 encryption\n  source: https://developer.bell.ca/faq/apis\n  evidence: >-\n    \"Security is maintained at all layers of the integration. Bell supports TLSv1.2, 256 bit SHA2\n    encryption and SSL with proactive monitoring of inbound and outbound traffic. Please ensure you\n    do not submit private data via the Sandbox API.\"\nnot_supported:\n  oauth2: true\n  openid_connect: true\n  ciba: true\n  mutual_tls: unknown\n  scopes: true\n  note: >-\n    No /.well-known/openid-configuration or /.well-known/oauth-authorization-server is served on\n    any Bell host probed (developer.bell.ca returns the Next.js HTML catch-all\
  \ with a 200 status;\n    www.bell.ca returns 404; api.bell.ca returns a JSON gateway 404). Because there is no OAuth\n    surface there is no scope catalogue, so scopes/ is intentionally absent for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/authentication/bell-canada-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Telecommunications
- Canada
- Mobile Network Operator
- Broadband
- 5G
- IoT
- TM Forum
- BSS
- OSS
- Network APIs
- CAMARA
- Open Gateway
- Identity Verification
- SIM Swap
- Enterprise
---
