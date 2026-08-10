---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Connected Kerb Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Connected Kerb secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Connected Kerb
provider_slug: connected-kerb
scheme_count: 3
schemes:
- description: OCPI Token-based authentication per the Open Charge Point Interface specification. Credentials are exchanged bilaterally through the OCPI credentials module rather than issued self-service; the endpoint rejects anonymous callers with an OCPI status envelope rather than a plain HTTP body.
  endpoints:
    credentials: https://cp.connectedkerb.com/ocpi/2.2.1/credentials
    versions: https://cp.connectedkerb.com/ocpi/versions
  evidence:
  - body: '{"status_code":2001,"status_message":"Unauthorized","timestamp":"2026-08-04T16:00:15Z"}'
    content_type: application/json
    http_status: 401
    response_headers:
    - OCPI-from-party-id
    - OCPI-from-country-code
    - OCPI-to-party-id
    - OCPI-to-country-code
    - X-Request-ID
    - X-Correlation-ID
    url: https://cp.connectedkerb.com/ocpi/versions
  - http_status: 401
    url: https://cp.connectedkerb.com/ocpi/2.2.1/credentials
  name: ocpiToken
  scheme: token
  surface: connected-kerb:ocpi
  type: http
- bearerFormat: API Token
  description: 'Long-lived UUID API token passed as `Authorization: Bearer <token>`. Tokens are created in the operator back office (API Access Tokens), scoped by an assigned role, and optionally restricted to whitelisted source IPs or to a single partner. There is no public sign-up path for API credentials.'
  evidence:
  - body: '{"message":"Unauthenticated."}'
    content_type: application/json
    http_status: 401
    response_headers:
    - 'X-App-Version: 3.225.1 (9e5dd506)'
    - x-req-trace-id
    url: https://cp.connectedkerb.com/public-api/resources/charge-points/v1.0
  name: bearerAuth
  scheme: bearer
  surface: connected-kerb:public-api
  type: http
- description: The platform contract documents an OAuth 2.0 client-credentials grant (RFC 6749 section 4.4) exchanging a hex client_secret at /public-api/oauth/token for a short-lived bearer access token, with an empty scopes map. It is NOT enabled on Connected Kerb's tenant - the token endpoint answers "Feature is not enabled" - so in practice the only working credential on this deployment is a long-lived bearer API token. That is the weaker of the two options the platform offers.
  evidence:
  - body: '{"message":"Feature is not enabled"}'
    http_status: 404
    method: POST
    url: https://cp.connectedkerb.com/public-api/oauth/token
  - http_status: 405
    method: GET
    url: https://cp.connectedkerb.com/public-api/oauth/token
  flows:
  - flow: clientCredentials
    scopes: {}
    tokenUrl: https://cp.connectedkerb.com/public-api/oauth/token
  name: oauth2ClientCredentials
  status: not-enabled-on-this-tenant
  surface: connected-kerb:public-api
  type: oauth2
slug: connected-kerb-authentication
source_filename: connected-kerb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: live probes of https://cp.connectedkerb.com + platform authorization\n  documentation at https://developers.ampeco.com/reference/authorization-1\ndocs: https://developers.ampeco.com/reference/authorization-1\nnote: |\n  Connected Kerb publishes no first-party developer portal, no authentication guide\n  and no OpenAPI, so there is nothing in this repo to derive a spec-based auth\n  profile from. This profile was assembled instead from (a) live unauthenticated\n  probes of the two API surfaces Connected Kerb actually operates on its own hosts\n  and (b) the published contract of the platform those surfaces run on. Every\n  status code below was observed, not assumed.\nsummary:\n  types: [http, oauth2]\n  api_key_in: []\n  http_schemes: [bearer, token]\n  oauth2_flows: [clientCredentials]\n  oauth2_enabled_on_this_tenant: false\n  self_service_credentials: false\n  credential_issuance: manual - commercial agreement or operator\
  \ back office\nschemes:\n- name: ocpiToken\n  surface: connected-kerb:ocpi\n  type: http\n  scheme: token\n  description: >-\n    OCPI Token-based authentication per the Open Charge Point Interface\n    specification. Credentials are exchanged bilaterally through the OCPI\n    credentials module rather than issued self-service; the endpoint rejects\n    anonymous callers with an OCPI status envelope rather than a plain HTTP body.\n  endpoints:\n    versions: https://cp.connectedkerb.com/ocpi/versions\n    credentials: https://cp.connectedkerb.com/ocpi/2.2.1/credentials\n  evidence:\n  - url: https://cp.connectedkerb.com/ocpi/versions\n    http_status: 401\n    content_type: application/json\n    body: '{\"status_code\":2001,\"status_message\":\"Unauthorized\",\"timestamp\":\"2026-08-04T16:00:15Z\"}'\n    response_headers: [OCPI-from-party-id, OCPI-from-country-code, OCPI-to-party-id,\n      OCPI-to-country-code, X-Request-ID, X-Correlation-ID]\n  - url: https://cp.connectedkerb.com/ocpi/2.2.1/credentials\n\
  \    http_status: 401\n- name: bearerAuth\n  surface: connected-kerb:public-api\n  type: http\n  scheme: bearer\n  bearerFormat: API Token\n  description: >-\n    Long-lived UUID API token passed as `Authorization: Bearer <token>`. Tokens are\n    created in the operator back office (API Access Tokens), scoped by an\n    assigned role, and optionally restricted to whitelisted source IPs or to a\n    single partner. There is no public sign-up path for API credentials.\n  evidence:\n  - url: https://cp.connectedkerb.com/public-api/resources/charge-points/v1.0\n    http_status: 401\n    content_type: application/json\n    body: '{\"message\":\"Unauthenticated.\"}'\n    response_headers: ['X-App-Version: 3.225.1 (9e5dd506)', x-req-trace-id]\n- name: oauth2ClientCredentials\n  surface: connected-kerb:public-api\n  type: oauth2\n  status: not-enabled-on-this-tenant\n  description: >-\n    The platform contract documents an OAuth 2.0 client-credentials grant (RFC 6749\n    section 4.4) exchanging\
  \ a hex client_secret at /public-api/oauth/token for a\n    short-lived bearer access token, with an empty scopes map. It is NOT enabled on\n    Connected Kerb's tenant - the token endpoint answers \"Feature is not enabled\" -\n    so in practice the only working credential on this deployment is a long-lived\n    bearer API token. That is the weaker of the two options the platform offers.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cp.connectedkerb.com/public-api/oauth/token\n    scopes: {}\n  evidence:\n  - url: https://cp.connectedkerb.com/public-api/oauth/token\n    method: POST\n    http_status: 404\n    body: '{\"message\":\"Feature is not enabled\"}'\n  - url: https://cp.connectedkerb.com/public-api/oauth/token\n    method: GET\n    http_status: 405\nother_gated_surfaces:\n- name: Customer portal\n  url: https://portal.connectedkerb.com/\n  auth: Microsoft Entra ID / MSAL browser sign-in (no anonymous API)\n  evidence:\n  - url: https://portal.connectedkerb.com/api/tenant/config\n\
  \    http_status: 401\n    body: '{\"error\":\"Unauthorized\"}'\n- name: Umbraco Delivery API (marketing site CMS)\n  url: https://www.connectedkerb.com/umbraco/delivery/api/v2/content\n  auth: API key required; not a published developer surface\n  evidence:\n  - url: https://www.connectedkerb.com/umbraco/delivery/api/v2/content\n    http_status: 401\n    content_type: application/problem+json\ngaps:\n- No Connected Kerb authentication documentation exists on any Connected Kerb host.\n- No self-service credential issuance for either API surface.\n- OAuth 2.0 client credentials is available in the platform but switched off on this\n  tenant, leaving long-lived bearer tokens as the only mechanism.\n- No scopes are defined for the OAuth flow even where it is enabled, so there is no\n  least-privilege scope surface to document (scopes/ is intentionally not emitted).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connected-kerb/refs/heads/main/authentication/connected-kerb-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- EV Charging
- Electric Vehicles
- Charge Point Operator
- Energy
- Transportation
- Smart Charging
- OCPI
- Roaming
- United Kingdom
- Infrastructure
- Sustainability
---
