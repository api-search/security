---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ch-robinson-worldwide-rest-apis-openapi.yml
  format: yaml
  label: C.H. Robinson Carrier API
  slug: carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-rest-apis-openapi.yml
- filename: ch-robinson-worldwide-rest-apis-openapi.yml
  format: yaml
  label: C.H. Robinson Navisphere Shipper API
  slug: shipper-navisphere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-rest-apis-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ch Robinson Worldwide Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: C.H. Robinson secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: C.H. Robinson
provider_slug: ch-robinson-worldwide
scheme_count: 2
schemes:
- applies_to: global security requirement in the contract
  bearerFormat: jwt
  name: sandbox
  scheme: bearer
  sources:
  - openapi/ch-robinson-worldwide-rest-apis-openapi.yml
  type: http
- applies_to: the four partner-implemented callback operations (Events Callback, Shipment Details Callback, Offer Response Callback, Load Documents Callback) - this is the token C.H. Robinson presents TO the partner
  bearerFormat: jwt
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ch-robinson-worldwide-rest-apis-openapi.yml
  type: http
slug: ch-robinson-worldwide-authentication
source_filename: ch-robinson-worldwide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/ch-robinson-worldwide-rest-apis-openapi.yml\ndocs: https://developer.chrobinson.com/api-reference#tag/Authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  self_service_signup: false\nmodel:\n  protocol: OAuth 2.0 (RFC 6749) client credentials\n  token_endpoint: https://api.navisphere.com/v1/oauth/token\n  sandbox_token_endpoint: https://sandbox-api.navisphere.com/v1/oauth/token\n  operation_id: Generate Token\n  request_body:\n    client_id: issued during onboarding\n    client_secret: issued during onboarding\n    audience: https://inavisphere.chrobinson.com\n    grant_type: client_credentials\n  content_types:\n  - application/json\n  - application/x-www-form-urlencoded\n  token_format: JWT\n  token_lifetime: 24 hours\n  presented_as: 'Authorization: Bearer <jwt>'\n  scopes: []\n  refresh: re-request with client credentials\n  provider_guidance: >-\n\
  \    The Authentication tag carries an explicit warning - \"Generated tokens are valid for 24 hours.\n    Users should only be hitting the C.H. Robinson authentication endpoint once every 24 hours.\n    Calling the authentication endpoint multiple times within the same 24 hour period may result\n    in users being subjected to rate limiting.\"\n  flow_diagram: https://api.navisphere.com/api/B2B/Portal/v1/documents/descriptions/Auth_flow.jpeg\n  code_samples:\n  - Curl\n  - Java\n  - NodeJS\n  - \"C#\"\nschemes:\n- name: sandbox\n  type: http\n  scheme: bearer\n  bearerFormat: jwt\n  applies_to: global security requirement in the contract\n  sources:\n  - openapi/ch-robinson-worldwide-rest-apis-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: jwt\n  applies_to: >-\n    the four partner-implemented callback operations (Events Callback, Shipment Details\n    Callback, Offer Response Callback, Load Documents Callback) - this is the token\n    C.H. Robinson presents\
  \ TO the partner\n  sources:\n  - openapi/ch-robinson-worldwide-rest-apis-openapi.yml\ngaps:\n  scopes_published: false\n  discovery_document: false\n  note: >-\n    No scopes are declared anywhere in the contract and no /.well-known/oauth-authorization-server\n    or /.well-known/openid-configuration is served, so authorization is all-or-nothing per\n    credential and cannot be discovered programmatically. No scopes/ artifact is emitted -\n    there is no scope surface to record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/authentication/ch-robinson-worldwide-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Freight
- Logistics
- Shipping
- Supply Chain
- Transportation
- Transportation Management
- Fortune 500
---
