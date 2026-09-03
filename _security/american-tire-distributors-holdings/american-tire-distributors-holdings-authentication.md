---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: American Tire Distributors Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: American Tire Distributors Holdings declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: American Tire Distributors Holdings
provider_slug: american-tire-distributors-holdings
scheme_count: 1
schemes:
- confidence: medium
  description: Every integrator guide instructs the operator to enter an "API key" and a "secret" supplied by ATD. The transport placement (header vs query vs body) is not stated in any public source, so it is recorded as unknown rather than guessed.
  evidence: 'Flxpoint: "input the API key, secret, and any other required information provided by ATD".'
  id: atd-api-key-secret
  in: unknown
  parameter_name: unknown
  scopes: []
  type: apiKey
slug: american-tire-distributors-holdings-authentication
source_filename: american-tire-distributors-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://help.flxpoint.com/en_US/automotive-part/american-tire-distributors-as-a-source\n  (Flxpoint integration guide, 302 -> flxpoint-p.helpjuice.com, HTTP 200);\n  https://dataheretothere.com/2024/11/23/connecting-atd-american-tire-distributors/ (HTTP 200);\n  https://www.sparkshipping.com/integrations/american-tire-distributors;\n  plus live probes of https://atdonline.com/login (200) and https://customer.atd-us.com/ (200).\nnote: >-\n  American Tire Distributors DOES operate a real partner API - integration platforms\n  (Flxpoint, Spark Shipping, InfiPlex, Finale Inventory, X-Cart, Data Here-to-There) all ship\n  a first-class ATD connector - but ATD publishes NO public developer portal, NO reference\n  documentation and NO machine-readable contract. Everything below is reconstructed from those\n  third-party integrator guides, which are consistent with each other; it is second-hand\n  evidence and is labelled as\
  \ such. ATD's own documentation is issued only to registered\n  dealers, and credentials are provisioned by an ATD representative by email\n  (integrator guidance names an @atd-us.com contact). No securityScheme could be derived\n  because no OpenAPI exists in this repo or on any ATD host.\ndocs: null\ndocs_status: not-published\napi_documented_publicly: false\ncredential_issuance:\n  process: manual\n  detail: >-\n    Requester must already be a registered ATD dealer (apply at https://atdonline.com/register).\n    API key and secret are issued by an ATD representative; there is no self-service key page\n    on any public ATD host.\n  self_service: false\n  signup_url: https://atdonline.com/register\nschemes:\n  - id: atd-api-key-secret\n    type: apiKey\n    confidence: medium\n    in: unknown\n    parameter_name: unknown\n    description: >-\n      Every integrator guide instructs the operator to enter an \"API key\" and a \"secret\"\n      supplied by ATD. The transport placement (header\
  \ vs query vs body) is not stated in any\n      public source, so it is recorded as unknown rather than guessed.\n    evidence: >-\n      Flxpoint: \"input the API key, secret, and any other required information provided by ATD\".\n    scopes: []\nenvironments:\n  - name: sandbox\n    purpose: >-\n      ATD requires a successful test order placed in Sandbox, and confirmed by ATD, before it\n      will enable Production ordering for an integration.\n    self_service: false\n    published_test_values: none\n    evidence: Flxpoint / Data Here-to-There integration guides.\n  - name: production\n    purpose: Live catalog, inventory, pricing, dropship ordering and shipment tracking.\n    self_service: false\n    gated_by: ATD confirmation of the sandbox test order.\noauth2: false\nopenid_connect: false\nmutual_tls: unknown\ncorporate_identity:\n  note: >-\n    Recorded for completeness and explicitly NOT an API auth surface. ATD's employee and\n    customer-portal SSO runs on an Okta tenant\
  \ (https://atd.okta.com); customer.atd-us.com\n    (ServiceNow) 302s unauthenticated requests into an Okta SAML flow. The discovery documents\n    served at atd.okta.com are Okta platform defaults describing Okta's own management API,\n    not an ATD contract - see well-known/american-tire-distributors-holdings-well-known.yml.\n  identity_provider: Okta\n  protocols_observed:\n    - SAML 2.0\n    - OpenID Connect\n  evidence_url: https://customer.atd-us.com/.well-known/openid-configuration\n  evidence_status: 302\ngaps:\n  - No public API reference or getting-started page on any atd.com / atdonline.com host.\n  - No OpenAPI, Swagger, GraphQL SDL, AsyncAPI, WSDL or .proto discoverable on any ATD host.\n  - Key placement, token lifetime, rotation policy and error responses are all undocumented publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-tire-distributors-holdings/refs/heads/main/authentication/american-tire-distributors-holdings-authentication.yml
summary_line: 1 scheme
tags:
- Tires
- Automotive
- Distribution
- Wholesale
- Supply Chain
- Logistics
---
