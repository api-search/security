---
api_key_in: []
api_specs:
- filename: mycarrier-public-api-openapi.json
  format: json
  label: MyCarrier Public API
  slug: mycarrier-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-public-api-openapi.json
- filename: mycarrier-order-public-api-openapi.json
  format: json
  label: MyCarrier Order API
  slug: mycarrier-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-order-public-api-openapi.json
- filename: mycarrier-freightaudit-api-openapi.json
  format: json
  label: MyCarrier FreightAudit API
  slug: mycarrier-freightaudit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-freightaudit-api-openapi.json
- filename: mycarrier-webhook-api-openapi.json
  format: json
  label: MyCarrier Webhook Registration API
  slug: mycarrier-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-webhook-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mycarrier Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyCarrier secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MyCarrier
provider_slug: mycarrier
scheme_count: 2
schemes:
- credential_location: Authorization header
  description: 'Basic Authorization: use `email` (account admin email) / `api-key` (Order API Key) for login.'
  docs: https://developer.mycarrier.io/docs/authentication-1
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/mycarrier-order-public-api-openapi.json
  - openapi/mycarrier-freightaudit-public-api-openapi.json
  - openapi/mycarrier-public-api-openapi.json
  type: http
- bearerFormat: JWT
  description: Enter JWT Bearer token only.
  name: Bearer
  scheme: bearer
  sources:
  - openapi/mycarrier-freightaudit-api-openapi.json
  - openapi/mycarrier-webhook-api-openapi.json
  type: http
slug: mycarrier-authentication
source_filename: mycarrier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://developer.mycarrier.io/docs/authentication-1\ndocs: https://developer.mycarrier.io/docs/authentication-1\nsummary:\n  types:\n  - http\n  primary: http-basic\n  note: 'MyCarrier''s documented public API uses HTTP Basic authentication. The username\n    is the email address of the account admin and the password is the Order API Key.\n    The FreightAudit live contract and the webhook-registration contract additionally\n    declare a Bearer JWT scheme. No OAuth 2.0, OpenID Connect or mTLS scheme is declared\n    in any published MyCarrier contract, so there is no scope surface and scopes/ is\n    intentionally absent.'\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: 'Basic Authorization: use `email` (account admin email) / `api-key`\n    (Order API Key) for login.'\n  credential_location: Authorization header\n  sources:\n  - openapi/mycarrier-order-public-api-openapi.json\n  - openapi/mycarrier-freightaudit-public-api-openapi.json\n\
  \  - openapi/mycarrier-public-api-openapi.json\n  docs: https://developer.mycarrier.io/docs/authentication-1\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter JWT Bearer token only.\n  sources:\n  - openapi/mycarrier-freightaudit-api-openapi.json\n  - openapi/mycarrier-webhook-api-openapi.json\nkey_management:\n  where: 'The API key is issued per customer account and read from the MyCarrier web\n    app under Customer Settings -> \"Order API Key\", which must be unmasked to reveal\n    it.'\n  docs: https://developer.mycarrier.io/docs/authentication-1\n  rotation_policy: not published\n  self_service_issuance: false\n  issuance_note: 'Keys are provisioned by MyCarrier. The docs direct customers to contact\n    support@mycarrier.io when the Order API Key field is blank, and sandbox access plus\n    an API key are set up by MyCarrier on request via https://go.mycarrier.io/sign-up.'\ntransport:\n  https_required: true\n  note: 'The docs state that\
  \ all API interactions must be over HTTPS and that HTTP\n    and unauthenticated requests will not succeed.'\ngaps:\n- 'The documented v1 Public API contract (openapi/mycarrier-public-api-openapi.json)\n  declares an EMPTY components.securitySchemes object and no top-level security[],\n  even though every operation documents a 401 response and the docs describe Basic\n  auth. The auth model is only discoverable from prose, not from that contract.'\n- No published key rotation or expiry policy.\n- No OAuth 2.0 / OIDC surface, so no delegated or scoped third-party access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/authentication/mycarrier-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Logistics
- Transportation
- Freight
- Shipping
- LTL
- Supply Chain
- Transportation Management
- Freight Audit
- Invoicing
---
