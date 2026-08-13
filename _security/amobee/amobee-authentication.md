---
api_key_in: []
api_specs:
- filename: amobee-services-openapi.json
  format: json
  label: Amobee Services Gateway API
  slug: amobee-services-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-services-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Amobee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amobee declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Amobee
provider_slug: amobee
scheme_count: 1
schemes:
- client_authentication: http_basic
  credential_issuance: Credentials are not self-service. Schedule A of the Master Service Terms states the API Client "will use the API through an API-only account created by Amobee" — an account is provisioned by Amobee under a signed agreement.
  evidence:
  - detail: 'Allow: POST — the endpoint is live and POST-only'
    observed: '2026-08-12'
    probe: GET https://services.amobee.com/accounts/v1/api/token
    status: 405
  - detail: '{"access_token":null,"token_type":null,"expires_in":null,"error":"invalid_request", "error_description":"Unable to parse authorization basic token."} — the server expects the client_id/client_secret pair in an HTTP Basic Authorization header'
    observed: '2026-08-12'
    probe: POST https://services.amobee.com/accounts/v1/api/token with grant_type=client_credentials and no credentials
    status: 400
  flow: clientCredentials
  id: oauth2_client_credentials
  scopes_documented: false
  scopes_note: No public scope reference is published. Do not confuse the Okta org scopes exposed at amobee-platform.okta.com/.well-known/openid-configuration with Amobee API scopes — those govern the Okta tenant, not the Platform API.
  token_endpoint: https://services.amobee.com/accounts/v1/api/token
  token_use: The issued access_token is presented as a Bearer token in the Authorization header on Amobee Platform API (campaign/v3) requests.
  type: oauth2
slug: amobee-authentication
source_filename: amobee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  live probes of https://services.amobee.com/accounts/v1/api/token plus the Amobee\n  Master Service Terms Schedule A (API Usage) at\n  https://www.amobee.com/trust/master-service-terms/schedule-a/\nnote: >-\n  Derived from what the live endpoint actually answers, not from a spec — the\n  Amobee Platform API reference (services.amobee.com/campaign/v3/doc/) now returns\n  404 and the help center is customer-gated, so no securitySchemes block was\n  available to derive from.\nschemes:\n  - id: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://services.amobee.com/accounts/v1/api/token\n    client_authentication: http_basic\n    evidence:\n      - probe: GET https://services.amobee.com/accounts/v1/api/token\n        status: 405\n        detail: 'Allow: POST — the endpoint is live and POST-only'\n        observed: '2026-08-12'\n      - probe: POST https://services.amobee.com/accounts/v1/api/token\
  \ with grant_type=client_credentials and no credentials\n        status: 400\n        detail: >-\n          {\"access_token\":null,\"token_type\":null,\"expires_in\":null,\"error\":\"invalid_request\",\n          \"error_description\":\"Unable to parse authorization basic token.\"} — the server expects the\n          client_id/client_secret pair in an HTTP Basic Authorization header\n        observed: '2026-08-12'\n    token_use: >-\n      The issued access_token is presented as a Bearer token in the Authorization\n      header on Amobee Platform API (campaign/v3) requests.\n    credential_issuance: >-\n      Credentials are not self-service. Schedule A of the Master Service Terms\n      states the API Client \"will use the API through an API-only account created\n      by Amobee\" — an account is provisioned by Amobee under a signed agreement.\n    scopes_documented: false\n    scopes_note: >-\n      No public scope reference is published. Do not confuse the Okta org scopes\n      exposed\
  \ at amobee-platform.okta.com/.well-known/openid-configuration with\n      Amobee API scopes — those govern the Okta tenant, not the Platform API.\nconsole_sso:\n  provider: Okta\n  tenant: https://amobee-platform.okta.com\n  preview_tenant: https://amobee-platform.oktapreview.com\n  console: https://platform.amobee.com/app/account/index.htm\n  discovered_via: Content-Security-Policy header on https://services.amobee.com/accounts/v1/api/token\n  evidence:\n    - url: https://amobee-platform.okta.com/.well-known/openid-configuration\n      status: 200\n    - url: https://platform.amobee.com/\n      status: 200\n  note: >-\n    Human operators sign in to the Amobee DSP console through an Okta-hosted SSO.\n    This is the UI login path, distinct from the machine-to-machine\n    client_credentials flow used by API clients.\ntransport:\n  tls: required\n  hsts_observed: 'strict-transport-security: max-age=15724800; includeSubDomains'\n  hsts_source: response headers from https://services.amobee.com/accounts/v1/api/token\n\
  docs:\n  reference: null\n  reference_note: >-\n    https://services.amobee.com/campaign/v3/doc/ (the URL apis.yml has carried as\n    the API documentation) returned HTTP 404 on 2026-08-12. help.amobee.com\n    returns 403 to anonymous requests and its Help Center API returns 401, so the\n    authentication guide is customer-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/authentication/amobee-authentication.yml
summary_line: 1 scheme
tags:
- Digital Advertising
- DSP
- Programmatic
- Campaign Management
- Audience Targeting
- Data Management Platform
- Ad Tech
- Samsung Ads
---
