---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Fasten Connect API
  slug: fasten-connect
  spec_type: OpenAPI
  url: https://docs.connect.fastenhealth.com/api-reference/openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fasten Health Authentication
name_suffix: Authentication
oauth_flows:
- pushed-authorization-request
overview: Fasten Health secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the pushed-authorization-request flow(s).
provider_name: Fasten Health
provider_slug: fasten-health
scheme_count: 3
schemes:
- applies_to: Fasten Connect REST API (https://api.connect.fastenhealth.com/v1)
  description: 'Basic Authentication containing an API Public ID and Private Key generated from the Fasten Connect Portal. The docs warn explicitly: do not expose these keys in the browser.'
  header: 'Authorization: Basic base64(public_id:private_key)'
  key_management: https://portal.fastenhealth.com
  key_modes:
  - description: Test mode key identifying your app.
    mode: test
    prefix: public_test_
    role: client-side
    secret: false
  - description: Test mode authenticated-request key.
    mode: test
    prefix: private_test_
    role: server-side
    secret: true
  - description: Live mode key identifying your app.
    mode: live
    prefix: public_live_
    role: client-side
    secret: false
  - description: Live mode authenticated-request key.
    mode: live
    prefix: private_live_
    role: server-side
    secret: true
  mode_selection: The key used determines whether the request runs in live or test mode; there is no mode header or parameter and one server URL serves both.
  name: bridge_basic
  operations_note: 'Only 5 of 12 operations declare security in the spec: GET /bridge/catalog/export, GET /bridge/org_connection/{orgConnectionId}, POST /bridge/vault_connection/revoke, POST /bridge/fhir/ehi-export and GET /bridge/fhir/ehi-export/{taskId}. The download operation GET /bridge/fhir/ehi-export/{taskId}/download/{fileId} declares NO security in the spec, yet the docs and the provider''s own Agent Skill both state it requires authentication — a contract/documentation mismatch on the operation that returns PHI.'
  operations_public: 7
  operations_requiring_auth: 5
  password: API Private Key
  scheme: basic
  scoping: None. A private key is all-or-nothing — there is no scope, permission or least-privilege model for API consumers, and the same credential that reads catalog metadata can request and download a patient's complete medical record.
  sources:
  - openapi/fasten-health-connect-openapi-original.yml
  - https://docs.connect.fastenhealth.com/api-reference/authentication
  type: http
  username: API Public ID
- applies_to: Bring Your Own Identity (BYOI) TEFCA IAS flow
  client_authentication: HTTP Basic with the Fasten public ID and private key
  description: A second, OAuth-based authentication surface used only in the BYOI identity-proofing flow. Fasten authenticates ITSELF to the integrator using a signed client assertion JWT (iss https://api.connect.fastenhealth.com, sub = the integrator's stable patient_id, aud = the registered Token Exchange endpoint, with exp/iat/nbf/jti replay constraints), and the integrator returns a CSP-issued OIDC ID Token.
  endpoint: POST https://identity.fastenhealth.com/oauth2/par
  flow: pushed-authorization-request
  jwks: https://identity.fastenhealth.com/jwks.json
  mutual: true
  name: fasten-identity-par
  probe:
    checked: '2026-08-14'
    result: identity.fastenhealth.com does not resolve in public DNS (NXDOMAIN).
  scopes:
  - openid
  - profile
  - email
  see: scopes/fasten-health-scopes.yml
  sources:
  - https://docs.connect.fastenhealth.com/identity-proofing/bring-your-own-identity
  spec_declared: false
  standards:
  - RFC 9126
  - RFC 8693
  - RFC 7523
  - OpenID Connect Core 1.0
  type: oauth2
- description: 'Not an API authentication scheme but the third credential an integrator must manage: the shared secret used to verify that a received webhook came from Fasten.'
  direction: inbound-to-integrator
  header: Webhook-Signature
  name: webhook-signature
  replay_protection: signed timestamp inside the signature
  secret_scope: per endpoint, and different between test and live
  secret_source: Signing Secret on the endpoint's Delivery Logs page in the Developer Portal
  see: asyncapi/fasten-health-webhooks.yml
  sources:
  - https://docs.connect.fastenhealth.com/webhooks/verification
  spec: Standard Webhooks (https://www.standardwebhooks.com/)
  type: hmac-signature
slug: fasten-health-authentication
source_filename: fasten-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/fasten-health-connect-openapi-original.yml\ndocs: https://docs.connect.fastenhealth.com/api-reference/authentication\nnote: >-\n  Baseline derived mechanically by 0-working/derive-authentication.py from the published OpenAPI\n  (one scheme: bridge_basic), then upgraded from the provider's authentication and introduction\n  reference pages, which document the key-prefix mode model, the client-side vs server-side key\n  split and the separate OAuth 2.0 identity surface that the spec does not describe at all.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [basic]\n  oauth2_flows: [pushed-authorization-request]\n  api_key_in: []\n  spec_declared_types: [http]\n\nschemes:\n  - name: bridge_basic\n    type: http\n    scheme: basic\n    applies_to: Fasten Connect REST API (https://api.connect.fastenhealth.com/v1)\n    username: API Public ID\n    password: API Private Key\n    header: 'Authorization: Basic base64(public_id:private_key)'\n\
  \    description: >-\n      Basic Authentication containing an API Public ID and Private Key generated from the Fasten\n      Connect Portal. The docs warn explicitly: do not expose these keys in the browser.\n    sources:\n      - openapi/fasten-health-connect-openapi-original.yml\n      - https://docs.connect.fastenhealth.com/api-reference/authentication\n    key_modes:\n      - {mode: test, role: client-side, prefix: public_test_, secret: false, description: \"Test mode key identifying your app.\"}\n      - {mode: test, role: server-side, prefix: private_test_, secret: true, description: \"Test mode authenticated-request key.\"}\n      - {mode: live, role: client-side, prefix: public_live_, secret: false, description: \"Live mode key identifying your app.\"}\n      - {mode: live, role: server-side, prefix: private_live_, secret: true, description: \"Live mode authenticated-request key.\"}\n    mode_selection: >-\n      The key used determines whether the request runs in live or test\
  \ mode; there is no mode header\n      or parameter and one server URL serves both.\n    scoping: >-\n      None. A private key is all-or-nothing — there is no scope, permission or least-privilege model\n      for API consumers, and the same credential that reads catalog metadata can request and\n      download a patient's complete medical record.\n    key_management: https://portal.fastenhealth.com\n    operations_requiring_auth: 5\n    operations_public: 7\n    operations_note: >-\n      Only 5 of 12 operations declare security in the spec: GET /bridge/catalog/export,\n      GET /bridge/org_connection/{orgConnectionId}, POST /bridge/vault_connection/revoke,\n      POST /bridge/fhir/ehi-export and GET /bridge/fhir/ehi-export/{taskId}. The download operation\n      GET /bridge/fhir/ehi-export/{taskId}/download/{fileId} declares NO security in the spec, yet\n      the docs and the provider's own Agent Skill both state it requires authentication — a\n      contract/documentation mismatch\
  \ on the operation that returns PHI.\n\n  - name: fasten-identity-par\n    type: oauth2\n    flow: pushed-authorization-request\n    applies_to: Bring Your Own Identity (BYOI) TEFCA IAS flow\n    spec_declared: false\n    endpoint: POST https://identity.fastenhealth.com/oauth2/par\n    client_authentication: HTTP Basic with the Fasten public ID and private key\n    jwks: https://identity.fastenhealth.com/jwks.json\n    scopes: [openid, profile, email]\n    standards: [RFC 9126, RFC 8693, RFC 7523, OpenID Connect Core 1.0]\n    description: >-\n      A second, OAuth-based authentication surface used only in the BYOI identity-proofing flow.\n      Fasten authenticates ITSELF to the integrator using a signed client assertion JWT\n      (iss https://api.connect.fastenhealth.com, sub = the integrator's stable patient_id, aud = the\n      registered Token Exchange endpoint, with exp/iat/nbf/jti replay constraints), and the\n      integrator returns a CSP-issued OIDC ID Token.\n    mutual: true\n\
  \    probe:\n      checked: '2026-08-14'\n      result: identity.fastenhealth.com does not resolve in public DNS (NXDOMAIN).\n    sources:\n      - https://docs.connect.fastenhealth.com/identity-proofing/bring-your-own-identity\n    see: scopes/fasten-health-scopes.yml\n\n  - name: webhook-signature\n    type: hmac-signature\n    direction: inbound-to-integrator\n    header: Webhook-Signature\n    spec: Standard Webhooks (https://www.standardwebhooks.com/)\n    secret_scope: per endpoint, and different between test and live\n    secret_source: Signing Secret on the endpoint's Delivery Logs page in the Developer Portal\n    replay_protection: signed timestamp inside the signature\n    description: >-\n      Not an API authentication scheme but the third credential an integrator must manage: the\n      shared secret used to verify that a received webhook came from Fasten.\n    sources:\n      - https://docs.connect.fastenhealth.com/webhooks/verification\n    see: asyncapi/fasten-health-webhooks.yml\n\
  \nclient_side_credential:\n  field: public-id\n  used_by: Stitch widget (<fasten-stitch-element public-id=\"...\">)\n  safe_in_browser: true\n  note: >-\n    The public ID is designed for browser exposure and identifies the app to the Stitch consent\n    widget. One Stitch quickstart sample shows a `pub_live_` prefix while the API reference\n    documents `public_live_`; the API reference is authoritative.\n\ngaps:\n  - No OAuth or scoped authorization for API consumers — Basic auth with a full-privilege key.\n  - No documented key rotation policy or key expiry.\n  - No MFA/JIT or short-lived credential option for API access (portal login gained 2FA on 2026-08-04).\n  - >-\n    The PHI download operation declares no security requirement in the OpenAPI despite requiring\n    authentication in practice.\n  - No OIDC discovery document is reachable on any Fasten host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fasten-health/refs/heads/main/authentication/fasten-health-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Healthcare
- FHIR
- Personal Health Record
- Electronic Medical Record
- Health Data Interoperability
- TEFCA
- EHI Export
- Patient Consent
- Self-Hosted
- Open Source
- HL7
- Healthcare Connectivity
---
