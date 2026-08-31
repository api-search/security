---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Overhaul Authentication
name_suffix: Authentication
oauth_flows: []
overview: Overhaul declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Overhaul
provider_slug: overhaul
scheme_count: 0
schemes: []
slug: overhaul-authentication
source_filename: overhaul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live probes of api.over-haul.com, app.over-haul.com and auth.over-haul.com\nstatus: not-publicly-documented\nnotes: >-\n  Overhaul publishes no public authentication documentation for its Shipment, Device, Risk Event, ETA or FraudWatch\n  APIs — there is no developer portal, no API reference and no auth guide on over-haul.com, help.over-haul.com or any\n  discoverable subdomain. What follows is recorded from anonymous probes ONLY; it is observed infrastructure\n  behaviour, not a provider claim, and it is deliberately NOT wired as a `type: Authentication` pointer in apis.yml\n  because the provider does not document authentication publicly.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  documented_publicly: false\nschemes: []\nobservations:\n- host: api.over-haul.com\n  finding: >-\n    Every anonymous request, at any path, returns HTTP 403 with body {\"message\":\"Forbidden\"} and\n    Content-Type application/json.\
  \ This response body and shape is the AWS API Gateway default for a request missing a\n    required API key or authorizer credential, which indicates a credential-gated gateway but does NOT identify the\n    scheme (x-api-key, Lambda authorizer, IAM SigV4 and Cognito/JWT authorizers all produce it).\n  http_status: 403\n  confidence: medium\n- host: auth.over-haul.com\n  finding: >-\n    Resolves via CNAME to prod-azureadb2c-ejbgg5fee0g4fadp.a03.azurefd.net (Microsoft Entra External ID / Azure AD B2C\n    behind Azure Front Door), indicating Overhaul runs an OIDC-capable identity provider for its customer\n    applications. TLS on the vanity hostname fails certificate verification anonymously, and Azure AD B2C serves its\n    OIDC discovery document only under a tenant/policy path, so no /.well-known/openid-configuration could be read.\n    Whether the customer-facing APIs accept tokens from this IdP is not observable anonymously.\n  confidence: low\n- host: app.over-haul.com\n  finding:\
  \ Single-page web application shell; the Overhaul Web Application login surface. No auth metadata exposed.\n  http_status: 200\n  confidence: high\nnext_steps:\n- Request the API reference and auth guide from Overhaul (support@ / https://www.over-haul.com/support) to upgrade\n  this artifact to method-searched with real securityScheme detail.\nx-evidence:\n- fetched: '2026-08-02'\n  url: https://api.over-haul.com/\n  http_status: 403\n  content_type: application/json\n- fetched: '2026-08-02'\n  url: https://app.over-haul.com/\n  http_status: 200\n  content_type: text/html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overhaul/refs/heads/main/authentication/overhaul-authentication.yml
summary_line: 0 schemes
tags:
- Supply Chain
- supply-chain-visibility
- Logistics
- Transportation
- cargo-security
- risk-management
- fraud-prevention
- cold-chain
- iot
- Track and Trace
- freight
- Compliance
---
