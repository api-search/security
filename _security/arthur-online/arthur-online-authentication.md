---
api_key_in: []
api_specs:
- filename: arthur-online-properties-openapi.yml
  format: yaml
  label: Arthur Properties API
  slug: arthur-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-properties-openapi.yml
- filename: arthur-online-units-openapi.yml
  format: yaml
  label: Arthur Units API
  slug: arthur-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-units-openapi.yml
- filename: arthur-online-tenancies-openapi.yml
  format: yaml
  label: Arthur Tenancies API
  slug: arthur-tenancies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-tenancies-openapi.yml
- filename: arthur-online-tenants-openapi.yml
  format: yaml
  label: Arthur Tenants API
  slug: arthur-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-tenants-openapi.yml
- filename: arthur-online-applicants-openapi.yml
  format: yaml
  label: Arthur Applicants API
  slug: arthur-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-applicants-openapi.yml
- filename: arthur-online-viewings-openapi.yml
  format: yaml
  label: Arthur Viewings API
  slug: arthur-viewings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-viewings-openapi.yml
- filename: arthur-online-maintenance-openapi.yml
  format: yaml
  label: Arthur Maintenance API
  slug: arthur-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-maintenance-openapi.yml
- filename: arthur-online-financials-openapi.yml
  format: yaml
  label: Arthur Financials API
  slug: arthur-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-financials-openapi.yml
- filename: arthur-online-assets-openapi.yml
  format: yaml
  label: Arthur Assets API
  slug: arthur-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-assets-openapi.yml
- filename: arthur-online-utilities-openapi.yml
  format: yaml
  label: Arthur Utilities API
  slug: arthur-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-utilities-openapi.yml
- filename: arthur-online-certificates-openapi.yml
  format: yaml
  label: Arthur Certificates API
  slug: arthur-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-certificates-openapi.yml
- filename: arthur-online-entities-openapi.yml
  format: yaml
  label: Arthur Entities API
  slug: arthur-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-entities-openapi.yml
- filename: arthur-online-conversations-openapi.yml
  format: yaml
  label: Arthur Conversations API
  slug: arthur-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-conversations-openapi.yml
- filename: arthur-online-tags-openapi.yml
  format: yaml
  label: Arthur Tags API
  slug: arthur-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-tags-openapi.yml
- filename: arthur-online-notes-openapi.yml
  format: yaml
  label: Arthur Notes API
  slug: arthur-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-notes-openapi.yml
- filename: arthur-online-types-openapi.yml
  format: yaml
  label: Arthur Types API
  slug: arthur-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-types-openapi.yml
auth_types:
- oauth2
description: 'Arthur API v2 uses a single security model: OAuth 2.0 Authorization Code with a bearer access token, plus a mandatory X-EntityID header naming the Arthur account the call is scoped to. There are no API keys, no scopes and no client-credentials flow. Credentials are not self-serve - a developer must be inside a paying Arthur account and ask Arthur support for API access before an OAuth application can be registered.'
kind: authentication
layout: security
method: searched
name: Arthur Online Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Arthur Online secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Arthur Online
provider_slug: arthur-online
scheme_count: 1
schemes:
- description: OAuth 2.0 Authorization Code flow (RFC 6749 section 4.1), cited explicitly in the Arthur documentation. Access tokens last 14 days, refresh tokens 21 days, authorization codes 15 minutes.
  flows:
  - authorizationUrl: https://auth.arthuronline.co.uk/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://auth.arthuronline.co.uk/oauth/token
    scopes: 0
    tokenUrl: https://auth.arthuronline.co.uk/oauth/token
  name: arthurOAuth
  sources:
  - openapi/arthur-online-applicants-openapi.yml
  - openapi/arthur-online-assets-openapi.yml
  - openapi/arthur-online-certificates-openapi.yml
  - openapi/arthur-online-conversations-openapi.yml
  - openapi/arthur-online-entities-openapi.yml
  - openapi/arthur-online-financials-openapi.yml
  - openapi/arthur-online-maintenance-openapi.yml
  - openapi/arthur-online-notes-openapi.yml
  - openapi/arthur-online-properties-openapi.yml
  - openapi/arthur-online-tags-openapi.yml
  - openapi/arthur-online-tenancies-openapi.yml
  - openapi/arthur-online-tenants-openapi.yml
  - openapi/arthur-online-types-openapi.yml
  - openapi/arthur-online-units-openapi.yml
  - openapi/arthur-online-utilities-openapi.yml
  - openapi/arthur-online-viewings-openapi.yml
  type: oauth2
slug: arthur-online-authentication
source_filename: arthur-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/ (16 documents) - derived security schemes, upgraded from the provider docs\ndocs: https://developer.arthuronline.co.uk/\ndocs_detail: >-\n  Arthur API public Postman collection, API > Getting Started > 1. Create Application,\n  2. Authentication, 3. Refresh Token; and API > Useful Information > Request Structure and Security.\ndescription: >-\n  Arthur API v2 uses a single security model: OAuth 2.0 Authorization Code with a bearer access\n  token, plus a mandatory X-EntityID header naming the Arthur account the call is scoped to.\n  There are no API keys, no scopes and no client-credentials flow. Credentials are not self-serve -\n  a developer must be inside a paying Arthur account and ask Arthur support for API access before\n  an OAuth application can be registered.\n\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  scopes_published: false\n  mandatory_headers: [Authorization,\
  \ X-EntityID]\n\nschemes:\n  - name: arthurOAuth\n    type: oauth2\n    description: >-\n      OAuth 2.0 Authorization Code flow (RFC 6749 section 4.1), cited explicitly in the Arthur\n      documentation. Access tokens last 14 days, refresh tokens 21 days, authorization codes 15 minutes.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.arthuronline.co.uk/oauth/authorize\n        tokenUrl: https://auth.arthuronline.co.uk/oauth/token\n        refreshUrl: https://auth.arthuronline.co.uk/oauth/token\n        scopes: 0\n    sources:\n      - openapi/arthur-online-applicants-openapi.yml\n      - openapi/arthur-online-assets-openapi.yml\n      - openapi/arthur-online-certificates-openapi.yml\n      - openapi/arthur-online-conversations-openapi.yml\n      - openapi/arthur-online-entities-openapi.yml\n      - openapi/arthur-online-financials-openapi.yml\n      - openapi/arthur-online-maintenance-openapi.yml\n      - openapi/arthur-online-notes-openapi.yml\n\
  \      - openapi/arthur-online-properties-openapi.yml\n      - openapi/arthur-online-tags-openapi.yml\n      - openapi/arthur-online-tenancies-openapi.yml\n      - openapi/arthur-online-tenants-openapi.yml\n      - openapi/arthur-online-types-openapi.yml\n      - openapi/arthur-online-units-openapi.yml\n      - openapi/arthur-online-utilities-openapi.yml\n      - openapi/arthur-online-viewings-openapi.yml\n\ntenancy_header:\n  name: X-EntityID\n  required: true\n  description: >-\n    The Arthur entity (account) the call is scoped to. Every request must carry it, including\n    reads. Records are only addressable inside their entity; an id from another entity returns 404.\n  discovery: 'GET /entities (operationId listEntities) returns the entities a token can address.'\n\nonboarding:\n  self_serve: false\n  steps:\n    - Be an authorised user inside a paying Arthur account.\n    - Contact Arthur support to be granted API access (https://support.arthuronline.co.uk/support/home).\n    -\
  \ In Arthur go to Settings > Your Account > OAuth Applications > Add Application.\n    - Supply name, description, website and an HTTPS callback URL.\n    - Arthur issues a client id and client secret.\n  signup_page: https://www.arthuronline.co.uk/connect/arthur-api\n\ntoken_lifecycle:\n  authorization_code_ttl: 15 minutes\n  access_token_ttl: 14 days\n  refresh_token_ttl: 21 days\n  token_request_encoding: application/x-www-form-urlencoded\n  grants: [authorization_code, refresh_token]\n  expiry_error:\n    status: 401\n    body: '{\"error\": \"expired_token\", \"message\": \"This token has expired.\"}'\n\nscopes:\n  published: false\n  note: >-\n    Arthur publishes no OAuth scopes. A token carries whatever the authorising Arthur user can see.\n    The real access control is organisational: Arthur recommends creating a separate Manager account\n    for third-party developers, and Enterprise accounts can set per-Manager permissions to narrow\n    what an integration can reach.\n\ndiscovery:\n\
  \  openid_configuration: 'https://auth.arthuronline.co.uk/.well-known/openid-configuration - 404 (probed 2026-07-26)'\n  oauth_authorization_server: 'https://auth.arthuronline.co.uk/.well-known/oauth-authorization-server - 404 (probed 2026-07-26)'\n\ntoken_handling_guidance:\n  source: Arthur API collection > Useful Information > Security > Securing API Tokens\n  practices:\n    - Establish a system for rotating passwords and tokens.\n    - Encrypt sensitive data and avoid decrypting it early in the process.\n    - Store user access tokens in a secure, encrypted location.\n    - Regenerate keys and tokens on any suspicion of compromise.\n\nrelated:\n  conventions: conventions/arthur-online-conventions.yml\n  errors: errors/arthur-online-problem-types.yml\n  conformance: conformance/arthur-online-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/authentication/arthur-online-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Real Estate
- United Kingdom
- Property Management
- PropTech
- Rentals
- Lettings
- Tenancy
- Maintenance
- Property Listings
- Social Housing
- Student Housing
- Block Management
---
