---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- http-signature
description: ''
kind: authentication
layout: security
method: searched
name: Flywire Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Flywire secures its APIs with apiKey, oauth2, and http-signature across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Flywire
provider_slug: flywire
scheme_count: 3
schemes:
- api: Flywire Payments API
  description: 'Per-application API key. Sent on every request as the X-Authentication-Key header alongside Content-Type: application/json. There is no scope surface, no expiry documented, and no rotation procedure published.'
  docs: https://developers.flywire.com/education/Content/api-basics.htm
  host: api-platform.flywire.com
  in: header
  name: ApiKeyAuth
  parameter_name: X-Authentication-Key
  registration: '"Registering an application is a manual process at the moment." Contact Flywire to register an application and receive an API Key plus a Shared Secret for validating notifications.'
  scoped: false
  sources:
  - docs
  type: apiKey
- api: Flywire Invoicing API
  description: 'OAuth 2.0 Client Credentials. Authorization is enforced on two independent axes and BOTH fail closed with a bodyless 403: the token must carry the scope for the resource and operation, AND the token must be scoped to the company in the :reference path segment. Permissions that belong to dashboard users rather than to applications are never granted to an application token, so some operations are unreachable through the API entirely.'
  docs: https://solutions.flywire.com/en/invoicing/invoicing-api
  flow: clientCredentials
  host: invoicing.flywire.com
  in: header
  name: OAuth2ClientCredentials
  parameter_name: Authorization
  scheme: Bearer
  scope_count: 16
  scoped: true
  scopes_ref: scopes/flywire-scopes.yml
  sources:
  - docs
  token_endpoint: https://api.flywire.com/oauth/token
  token_request: JSON body with grant_type=client_credentials, client_id, client_secret
  token_response: access_token plus its time-to-live in seconds
  type: oauth2
- algorithm: base64(HMAC-SHA256(request body, shared secret))
  api: Flywire Payment Request API
  description: Request-level HMAC digest rather than a bearer credential. The digest is computed over the request body — or, for DELETE, over the payment request ID — using a shared secret arranged with Flywire. This is the same header name and algorithm Flywire uses to sign OUTBOUND webhook callbacks, used here in the inbound direction.
  docs: https://solutions.flywire.com/en/payment-requests/payment-request-api
  host: app.flywire.com
  in: header
  name: FlywireDigest
  parameter_name: X-Flywire-Digest
  scoped: false
  sources:
  - docs
  type: http-signature
slug: flywire-authentication
source_filename: flywire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://developers.flywire.com/education/Content/api-basics.htm\ndocs:\n- https://developers.flywire.com/education/Content/api-basics.htm\n- https://solutions.flywire.com/en/invoicing/invoicing-api\n- https://solutions.flywire.com/en/payment-requests/payment-request-api\nnotes: >-\n  Flywire publishes no OpenAPI on any host, so this profile is SEARCHED from the\n  developer documentation rather than derived from securitySchemes. The headline\n  finding is that Flywire runs THREE DIFFERENT AUTHORIZATION MODELS across three\n  public APIs, documented on two unconnected documentation estates, with no shared\n  credential and no discovery document tying them together. An integrator who\n  reads developers.flywire.com learns only about the static API-key header and\n  would have no way to know that the Invoicing API speaks OAuth 2.0. Probed\n  2026-09-02: /.well-known/oauth-authorization-server, /.well-known/openid-configuration\n\
  \  and /.well-known/oauth-protected-resource return 404 on www.flywire.com,\n  api.flywire.com, invoicing.flywire.com, app.flywire.com, app.demo.flywire.com,\n  api-platform.flywire.com, api-platform-sandbox.flywire.com and\n  developers.flywire.com — every scheme below must be learned from prose.\nsummary:\n  types: [apiKey, oauth2, http-signature]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  discovery_documents: []\n  models_count: 3\nschemes:\n- name: ApiKeyAuth\n  api: Flywire Payments API\n  host: api-platform.flywire.com\n  type: apiKey\n  in: header\n  parameter_name: X-Authentication-Key\n  description: >-\n    Per-application API key. Sent on every request as the X-Authentication-Key\n    header alongside Content-Type: application/json. There is no scope surface,\n    no expiry documented, and no rotation procedure published.\n  registration: >-\n    \"Registering an application is a manual process at the moment.\" Contact\n    Flywire to register an application\
  \ and receive an API Key plus a Shared\n    Secret for validating notifications.\n  scoped: false\n  sources: [docs]\n  docs: https://developers.flywire.com/education/Content/api-basics.htm\n- name: OAuth2ClientCredentials\n  api: Flywire Invoicing API\n  host: invoicing.flywire.com\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: https://api.flywire.com/oauth/token\n  token_request: JSON body with grant_type=client_credentials, client_id, client_secret\n  token_response: access_token plus its time-to-live in seconds\n  in: header\n  parameter_name: Authorization\n  scheme: Bearer\n  description: >-\n    OAuth 2.0 Client Credentials. Authorization is enforced on two independent\n    axes and BOTH fail closed with a bodyless 403: the token must carry the scope\n    for the resource and operation, AND the token must be scoped to the company in\n    the :reference path segment. Permissions that belong to dashboard users rather\n    than to applications are never granted to an\
  \ application token, so some\n    operations are unreachable through the API entirely.\n  scoped: true\n  scopes_ref: scopes/flywire-scopes.yml\n  scope_count: 16\n  sources: [docs]\n  docs: https://solutions.flywire.com/en/invoicing/invoicing-api\n- name: FlywireDigest\n  api: Flywire Payment Request API\n  host: app.flywire.com\n  type: http-signature\n  in: header\n  parameter_name: X-Flywire-Digest\n  algorithm: base64(HMAC-SHA256(request body, shared secret))\n  description: >-\n    Request-level HMAC digest rather than a bearer credential. The digest is\n    computed over the request body — or, for DELETE, over the payment request ID —\n    using a shared secret arranged with Flywire. This is the same header name and\n    algorithm Flywire uses to sign OUTBOUND webhook callbacks, used here in the\n    inbound direction.\n  scoped: false\n  sources: [docs]\n  docs: https://solutions.flywire.com/en/payment-requests/payment-request-api\nwebhook_auth:\n  header: X-Flywire-Digest\n  algorithm:\
  \ base64-encoded HMAC-SHA256 hash of the message body and a shared secret\n  secret: Shared Secret issued at application registration / arranged with your account manager\n  direction: inbound-to-your-endpoint\n  note: >-\n    Flywire signs callbacks with the same header and algorithm it accepts on the\n    Payment Request API. Verify the digest before trusting a callback body.\n  docs: https://solutions.flywire.com/en/webhooks/notifications-v2\ngaps:\n- No OAuth authorization-server metadata or OpenID configuration is served on any Flywire host (all probes 404, 2026-09-02).\n- No token expiry, rotation or revocation policy is published for the Payments API static key.\n- The three authorization models are documented on two separate doc sites that do not cross-link their auth sections.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flywire/refs/heads/main/authentication/flywire-authentication.yml
summary_line: apiKey/oauth2/http-signature · 3 schemes
tags:
- Company
- Payments
- Cross-Border Payments
- Fintech
- Education Payments
- Healthcare Payments
- Travel Payments
- B2B Payments
- Checkout
- Webhook
---
