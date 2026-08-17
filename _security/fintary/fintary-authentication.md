---
api_key_in:
- header
api_specs:
- filename: fintary-open-api-openapi.yml
  format: yaml
  label: Fintary Open API
  slug: fintary-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-open-api-openapi.yml
- filename: fintary-ams-api-openapi.yml
  format: yaml
  label: Fintary AMS API
  slug: fintary-ams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-ams-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fintary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fintary secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fintary
provider_slug: fintary
scheme_count: 2
schemes:
- applies_to: Fintary Open API, Fintary AMS API
  bearerFormat: string
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/fintary-ams-api-openapi.yml
  - openapi/fintary-open-api-openapi.yml
  type: http
- applies_to: Fintary Open API
  description: API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/fintary-open-api-openapi.yml
  type: apiKey
slug: fintary-authentication
source_filename: fintary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/fintary-ams-api-openapi.yml, openapi/fintary-open-api-openapi.yml\ndocs: https://api.fintary.com/documentation\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: string\n  sources:\n  - openapi/fintary-ams-api-openapi.yml\n  - openapi/fintary-open-api-openapi.yml\n  applies_to: Fintary Open API, Fintary AMS API\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authentication\n  sources:\n  - openapi/fintary-open-api-openapi.yml\n  applies_to: Fintary Open API\napplication:\n  style: global\n  note: >-\n    Both documents declare a top-level `security` requirement rather than per-operation\n    security. The Open API accepts either scheme (`ApiKeyAuth` OR `BearerAuth`); the AMS API\n    declares `BearerAuth` only. No operation in either document opts out.\nobserved:\n- url:\
  \ https://api.fintary.com/openapi/agents\n  status: 401\n  body: '{\"success\":false,\"data\":null,\"message\":\"Missing or invalid API key\",\"statusCode\":401}'\n  note: Confirms the x-api-key scheme is enforced live.\n- url: https://api.fintary.com/api/ams/agents\n  status: 401\n  body: Not authenticated\n  note: Confirms the AMS bearer scheme is enforced live.\nkey_issuance:\n  self_service: false\n  note: >-\n    Fintary publishes no key-management or token-issuance documentation. There is no\n    developer console, no key page, no signup, and no documented token endpoint for the\n    APIs themselves. Keys and bearer tokens are obtained through a Fintary representative\n    against an existing customer account.\nscopes:\n  published: false\n  note: >-\n    Neither document declares an oauth2 securityScheme and no scope or permission reference\n    is published, so no scopes/ artifact is emitted. Authorization is expressed instead as\n    coarse account roles - `account_admin`, `producer`,\
  \ `data_specialist` (named in the SSO\n    guides) - plus per-operation admin gates in the Open API, where `account_id` and\n    `contact_id` overrides are documented as \"Fintary Admin only\" or \"Fintary Admin or\n    Account Admin\".\nsso:\n  role: client\n  protocol: OAuth 2.0 authorization code\n  docs: https://api.fintary.com/documentation\n  self_service: false\n  note: >-\n    Distinct from API authentication. Fintary acts as the OAuth CLIENT against a customer's\n    identity provider: the user is redirected to the customer's authorization URL, the IdP\n    returns a code to Fintary's redirect URI, Fintary exchanges it at the customer's token\n    endpoint using client credentials the customer issues, then decodes the selected JWT and\n    reads claims. Fintary publishes no authorization server of its own and issues no\n    developer-facing scopes. Setup is performed by Fintary staff from configuration the\n    customer supplies.\n  variants:\n  - id: contact-sync-id-sso\n   \
  \ title: Contact Sync ID SSO\n    user_resolution: contact_sync_id\n    identity_claim: contact_id\n    role_claim: role\n    token_source: access_token or id_token\n    role_mapping: [account_admin, producer, data_specialist]\n    provisioning_flags: [createContactIfMissing, createUserIfMissing]\n    fallback: >-\n      userResolution.identityFallback = 'email' resolves the user by verified email when the\n      identity claim is absent; that path matches existing `users` records only and never\n      reads or writes `contacts`.\n    forwarded_entry: https://api.fintary.com/oauth/callback?code=<code>&provider=<provider_slug>\n  - id: email-sso\n    title: Email-based SSO\n    user_resolution: email\n    identity_claim: email\n    token_source: id_token first, falling back to access_token\n    provisioning: >-\n      Does not create users on the fly - users must be invited into Fintary in advance and\n      must be active, or login fails.\n  configuration_inputs:\n  - provider name/slug\n\
  \  - Fintary account (customer tenant) to map\n  - authorization URL\n  - token URL\n  - client ID and secret\n  - redirect URI(s)\n  - scopes and extra authorization parameters\n  - token endpoint content type (application/json or application/x-www-form-urlencoded)\ntransport:\n  https_only: true\n  hsts: 'max-age=63072000; includeSubDomains'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/authentication/fintary-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Fintech
- Insurance
- Insurtech
- Commissions
- Revenue Operations
- Analytics
- Agency Management
- Policy Management
- Payouts
- Reconciliation
- OpenAPI
---
