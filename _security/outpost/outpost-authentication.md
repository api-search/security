---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Outpost Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Outpost secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Outpost
provider_slug: outpost
scheme_count: 2
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  refresh: Cache token with expires_in - 300s buffer; refresh on expiry or on 401.
  source: https://outpostnow.com/docs/api/tax-of-record/
  tokenUrl: https://access.outpostanywhere.com/oauth2/token
  token_format: JWT
  token_ttl_seconds: 86400
  token_type: Bearer
  type: oauth2
  used_by:
  - Outpost Tax of Record API
  - Outpost Merchant of Record API
- bearerFormat: JWT
  credential_management: Client ID and secret created/rotated in the Partner Portal; up to 2 active API credentials at a time for safe key rotation.
  header: 'Authorization: Bearer <token>'
  name: PartnerBearerJWT
  scheme: bearer
  source: https://outpostnow.com/docs/api/hosted-onboarding/
  type: http
  used_by:
  - Outpost Hosted Onboarding (Partner) API
slug: outpost-authentication
source_filename: outpost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://outpostnow.com/docs/api/tax-of-record/\ndocs:\n- https://outpostnow.com/docs/api/tax-of-record/\n- https://outpostnow.com/docs/api/merchant-of-record/\n- https://outpostnow.com/docs/api/hosted-onboarding/\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  http_schemes:\n  - bearer\n  notes: >-\n    Tax of Record and Merchant of Record APIs use OAuth2 client-credentials\n    (server-to-server); the merchant's backend exchanges a client_id/client_secret\n    for a Bearer JWT access token. Hosted Onboarding (Partner) API authenticates\n    with a JWT Bearer token whose credentials are created and rotated in the\n    Partner Portal (up to 2 active credentials). Secrets are server-only and must\n    never be exposed to browsers or logs.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  used_by:\n  - Outpost Tax of Record API\n  - Outpost Merchant of Record API\n  flow: clientCredentials\n\
  \  tokenUrl: https://access.outpostanywhere.com/oauth2/token\n  grant_type: client_credentials\n  token_type: Bearer\n  token_format: JWT\n  token_ttl_seconds: 86400\n  refresh: Cache token with expires_in - 300s buffer; refresh on expiry or on 401.\n  source: https://outpostnow.com/docs/api/tax-of-record/\n- name: PartnerBearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  used_by:\n  - Outpost Hosted Onboarding (Partner) API\n  header: 'Authorization: Bearer <token>'\n  credential_management: >-\n    Client ID and secret created/rotated in the Partner Portal; up to 2 active\n    API credentials at a time for safe key rotation.\n  source: https://outpostnow.com/docs/api/hosted-onboarding/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outpost/refs/heads/main/authentication/outpost-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Merchant of Record
- Tax of Record
- Cross-Border Commerce
- Payments
- Tax Compliance
- E-Commerce
- VAT
- Fintech
- Invoicing
- Onboarding
---
