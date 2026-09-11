---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication profile for the Advisr REST API, read from the public API reference. Advisr uses a single company-scoped API token supplied in a custom `token` request header. There is no OAuth 2.0, OpenID Connect, mTLS or HTTP Basic surface, and no self-service key issuance — tokens are provisioned by an Advisr support representative for the customer company.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Advisr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Advisr declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Advisr
provider_slug: advisr
scheme_count: 1
schemes:
- applies_to: All Advisr API endpoints.
  description: Company access token. Sent verbatim as the `token` header on every request — there is no `Bearer` or other scheme prefix.
  docs: https://apidocs.advisr.com/#authentication
  example_shape: 'token: api-token'
  id: company_token
  in: header
  name: token
  type: apiKey
slug: advisr-authentication
source_filename: advisr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: https://apidocs.advisr.com/#authentication\ndescription: >-\n  Authentication profile for the Advisr REST API, read from the public API\n  reference. Advisr uses a single company-scoped API token supplied in a custom\n  `token` request header. There is no OAuth 2.0, OpenID Connect, mTLS or HTTP\n  Basic surface, and no self-service key issuance — tokens are provisioned by an\n  Advisr support representative for the customer company.\nbase_url: https://api.advisr.com/v1\nschemes:\n  - id: company_token\n    type: apiKey\n    in: header\n    name: token\n    description: >-\n      Company access token. Sent verbatim as the `token` header on every\n      request — there is no `Bearer` or other scheme prefix.\n    example_shape: 'token: api-token'\n    applies_to: All Advisr API endpoints.\n    docs: https://apidocs.advisr.com/#authentication\nscope_model:\n  type: none\n  detail: >-\n    The token is scoped to a company; the API\
  \ publishes no OAuth scopes,\n    permissions matrix or per-endpoint grant list. A 403 AdvisrPermissionError\n    is documented for a token that lacks the necessary permissions, so\n    server-side permissioning exists but is not documented as an addressable\n    scope surface.\nissuance:\n  self_service: false\n  how: >-\n    \"In order to retrieve your Company's access token please contact your\n    Support representative.\" Access to the API itself is also gated —\n    \"Please reach out to your account manager to inquire about access.\"\n  docs: https://apidocs.advisr.com/#introduction\nrotation:\n  documented: false\n  note: No key rotation, expiry or revocation procedure is published.\ntransport:\n  tls_required: true\n  note: All documented examples use https://api.advisr.com.\nfailure_modes:\n  - status: 401\n    type: AdvisrUnauthorizedError\n    meaning: Invalid or no API key provided for this request.\n  - status: 403\n    type: AdvisrPermissionError\n    meaning: The API key\
  \ used for this request does not have the necessary permissions.\ngaps:\n  - No OAuth 2.0 / OpenID Connect surface, so no delegated or per-user authorization.\n  - No documented token rotation, expiry, or revocation.\n  - Token issuance is a human support request, not an API or console flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advisr/refs/heads/main/authentication/advisr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Advertising
- Media
- Sales
- Sales Enablement
- Media Planning
- Proposals
- Advertising Sales
- Campaigns
- CRM
---
