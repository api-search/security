---
api_key_in: []
api_specs:
- filename: lever-webhooks-asyncapi.yml
  format: yaml
  label: Lever Webhooks
  slug: lever-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-webhooks-asyncapi.yml
- filename: lever-co-applications-api-openapi.yml
  format: yaml
  label: Lever Applications API
  slug: lever-co-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-applications-api-openapi.yml
- filename: lever-co-archive-reasons-api-openapi.yml
  format: yaml
  label: Lever Archive Reasons API
  slug: lever-co-archive-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-archive-reasons-api-openapi.yml
- filename: lever-co-audit-events-api-openapi.yml
  format: yaml
  label: Lever Audit Events API
  slug: lever-co-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-audit-events-api-openapi.yml
- filename: lever-co-eeo-responses-api-openapi.yml
  format: yaml
  label: Lever EEO Responses API
  slug: lever-co-eeo-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-eeo-responses-api-openapi.yml
- filename: lever-co-feedback-api-openapi.yml
  format: yaml
  label: Lever Feedback API
  slug: lever-co-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-feedback-api-openapi.yml
- filename: lever-co-files-api-openapi.yml
  format: yaml
  label: Lever Files API
  slug: lever-co-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-files-api-openapi.yml
- filename: lever-co-interviews-api-openapi.yml
  format: yaml
  label: Lever Interviews API
  slug: lever-co-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-interviews-api-openapi.yml
- filename: lever-co-notes-api-openapi.yml
  format: yaml
  label: Lever Notes API
  slug: lever-co-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-notes-api-openapi.yml
- filename: lever-co-offers-api-openapi.yml
  format: yaml
  label: Lever Offers API
  slug: lever-co-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-offers-api-openapi.yml
- filename: lever-co-opportunities-api-openapi.yml
  format: yaml
  label: Lever Opportunities API
  slug: lever-co-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-opportunities-api-openapi.yml
- filename: lever-co-panels-api-openapi.yml
  format: yaml
  label: Lever Panels API
  slug: lever-co-panels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-panels-api-openapi.yml
- filename: lever-co-postings-api-openapi.yml
  format: yaml
  label: Lever Postings API
  slug: lever-co-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-postings-api-openapi.yml
- filename: lever-co-requisitions-api-openapi.yml
  format: yaml
  label: Lever Requisitions API
  slug: lever-co-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-requisitions-api-openapi.yml
- filename: lever-co-sources-api-openapi.yml
  format: yaml
  label: Lever Sources API
  slug: lever-co-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-sources-api-openapi.yml
- filename: lever-co-stages-api-openapi.yml
  format: yaml
  label: Lever Stages API
  slug: lever-co-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-stages-api-openapi.yml
- filename: lever-co-tags-api-openapi.yml
  format: yaml
  label: Lever Tags API
  slug: lever-co-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-tags-api-openapi.yml
- filename: lever-co-users-api-openapi.yml
  format: yaml
  label: Lever Users API
  slug: lever-co-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-users-api-openapi.yml
- filename: lever-co-webhooks-api-openapi.yml
  format: yaml
  label: Lever Webhooks API
  slug: lever-co-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: Lever runs two distinct credential models against the same Data API base (https://api.lever.co/v1). HTTP Basic with an API key is for a customer's own internal workflows; OAuth 2.0 authorization code is the ONLY path for a third-party product integration and requires the app to be registered through the Lever partner program. All requests must be HTTPS; unencrypted HTTP is rejected.
kind: authentication
layout: security
method: searched
name: Lever Co Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lever secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lever
provider_slug: lever-co
scheme_count: 2
schemes:
- audience: Lever customers building their own internal workflows
  description: HTTP Basic authentication with the Lever API key as the USERNAME and an EMPTY password. Keys are created and revoked on the API Credentials tab of the Integrations and API page in Lever account settings. Multiple keys can be active at once; each key carries its own endpoint permissions and an optional confidential-data grant that can only be given at key creation.
  key_management_url: https://hire.lever.co/developer/documentation
  name: BasicAuth
  notes:
  - Lever does not issue API keys for partner integration development — OAuth is required.
  - Older Basic Auth integrations require the customer to hold the Data API feature.
  scheme: basic
  scoped: false
  sources:
  - https://hire.lever.co/developer/documentation
  type: http
- audience: Registered partner product integrations (mandatory since 2020)
  consent:
    granted_by: Lever Super Admin, on behalf of the whole organization
    re_consent: Consent is re-requested only on first authorization, after revocation, or when new scopes are requested.
    revocable: true
    revoke_location: The customer's Lever settings page lists the connected app and can revoke it.
  flows:
  - access_token_lifetime_seconds: 3600
    audience: https://api.lever.co/v1/
    authorizationUrl: https://auth.lever.co/authorize
    flow: authorizationCode
    refresh_tokens: Request the offline_access scope to receive a refresh_token; refresh returns a new access AND refresh token.
    required_params:
    - client_id
    - redirect_uri
    - response_type
    - state
    - audience
    - scope
    sandbox_audience: https://api.sandbox.lever.co/v1/
    sandbox_authorizationUrl: https://sandbox-lever.auth0.com/authorize
    scope_detail: scopes/lever-co-scopes.yml
    scope_limits: Most use cases need 5-8 scopes; hard maximum of 20 scopes per app. A write:admin scope implies the matching read:admin.
    tokenUrl: https://auth.lever.co/oauth/token
    token_type: Bearer
  name: OAuth2
  registration: Apps must be registered with Lever (name, 20-140 char description, callback URI(s), square 150x150 logo URI, requested scopes). Lever's team issues the client_id and client_secret. Sandbox and production are separate apps with separate callbacks.
  sources:
  - https://hire.lever.co/developer/oauth
  - https://hire.lever.co/developer/documentation
  type: oauth2
slug: lever-co-authentication
source_filename: lever-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://hire.lever.co/developer/documentation (Authentication section) and\n  https://hire.lever.co/developer/oauth, both fetched 2026-08-26 (HTTP 200).\n  Baseline derived from openapi/*.yml securitySchemes with\n  0-working/derive-authentication.py, then upgraded from the published docs.\ndocs:\n  - https://hire.lever.co/developer/documentation\n  - https://hire.lever.co/developer/oauth\ndescription: >-\n  Lever runs two distinct credential models against the same Data API base\n  (https://api.lever.co/v1). HTTP Basic with an API key is for a customer's own\n  internal workflows; OAuth 2.0 authorization code is the ONLY path for a\n  third-party product integration and requires the app to be registered through\n  the Lever partner program. All requests must be HTTPS; unencrypted HTTP is\n  rejected.\nbase_url: https://api.lever.co/v1\nsandbox_base_url: https://api.sandbox.lever.co/v1\neu_note: >-\n  Lever operates an\
  \ EU data centre. OAuth authorization and API actions for EU\n  customers are redirected automatically to the appropriate data centre; the\n  public Postings API has an EU host at https://api.eu.lever.co/v0/postings.\nsummary:\n  types:\n    - http\n    - oauth2\n  oauth2_flows:\n    - authorizationCode\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    audience: Lever customers building their own internal workflows\n    description: >-\n      HTTP Basic authentication with the Lever API key as the USERNAME and an\n      EMPTY password. Keys are created and revoked on the API Credentials tab of\n      the Integrations and API page in Lever account settings. Multiple keys can\n      be active at once; each key carries its own endpoint permissions and an\n      optional confidential-data grant that can only be given at key creation.\n    key_management_url: https://hire.lever.co/developer/documentation\n    scoped: false\n    notes:\n      - Lever does not issue API keys\
  \ for partner integration development — OAuth is required.\n      - Older Basic Auth integrations require the customer to hold the Data API feature.\n    sources:\n      - https://hire.lever.co/developer/documentation\n  - name: OAuth2\n    type: oauth2\n    audience: Registered partner product integrations (mandatory since 2020)\n    registration: >-\n      Apps must be registered with Lever (name, 20-140 char description, callback\n      URI(s), square 150x150 logo URI, requested scopes). Lever's team issues the\n      client_id and client_secret. Sandbox and production are separate apps with\n      separate callbacks.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.lever.co/authorize\n        tokenUrl: https://auth.lever.co/oauth/token\n        sandbox_authorizationUrl: https://sandbox-lever.auth0.com/authorize\n        required_params: [client_id, redirect_uri, response_type, state, audience, scope]\n        audience: https://api.lever.co/v1/\n\
  \        sandbox_audience: https://api.sandbox.lever.co/v1/\n        token_type: Bearer\n        access_token_lifetime_seconds: 3600\n        refresh_tokens: Request the offline_access scope to receive a refresh_token; refresh returns a new access AND refresh token.\n        scope_detail: scopes/lever-co-scopes.yml\n        scope_limits: Most use cases need 5-8 scopes; hard maximum of 20 scopes per app. A write:admin scope implies the matching read:admin.\n    consent:\n      granted_by: Lever Super Admin, on behalf of the whole organization\n      revocable: true\n      revoke_location: The customer's Lever settings page lists the connected app and can revoke it.\n      re_consent: Consent is re-requested only on first authorization, after revocation, or when new scopes are requested.\n    sources:\n      - https://hire.lever.co/developer/oauth\n      - https://hire.lever.co/developer/documentation\ncommon_failures:\n  - symptom: Consent screen shows only `offline_access`\n    cause:\
  \ The `audience` parameter is missing or malformed on /authorize.\n    fix: Pass audience=https://api.lever.co/v1/ (trailing slash required); sandbox uses https://api.sandbox.lever.co/v1/.\n  - symptom: 401 Unauthorized on token exchange\n    cause: The client SECRET was not used for client_secret (the API key was sent instead).\n    fix: Use the OAuth client_secret issued at app registration.\n  - symptom: 403 \"Unable to find a signing key that matches\"\n    cause: A sandbox token was presented to the production API (or vice versa).\n    fix: Match token issuer to base URL — https://api.sandbox.lever.co/v1 for sandbox, https://api.lever.co/v1 for production.\n  - symptom: Redirect window shows \"undefined\"\n    cause: A parameter in the redirect URL does not match the registered app, most often redirect_uri.\n    fix: Make redirect_uri byte-identical to the registered callback.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/authentication/lever-co-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Applicant Tracking
- ATS
- CRM
- Recruiting
- Hiring
- Talent Acquisition
- Human Resources
- HR Tech
- Postings
- Webhook
- Authentication
---
