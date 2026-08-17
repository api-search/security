---
api_key_in: []
api_specs:
- filename: google-ads-ad-groups-api-openapi.yml
  format: yaml
  label: Google Ads Ad Groups API
  slug: google-ads-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-ad-groups-api-openapi.yml
- filename: google-ads-ads-api-openapi.yml
  format: yaml
  label: Google Ads Ads API
  slug: google-ads-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-ads-api-openapi.yml
- filename: google-ads-bidding-strategies-api-openapi.yml
  format: yaml
  label: Google Ads Bidding Strategies API
  slug: google-ads-bidding-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-bidding-strategies-api-openapi.yml
- filename: google-ads-campaigns-api-openapi.yml
  format: yaml
  label: Google Ads Campaigns API
  slug: google-ads-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-campaigns-api-openapi.yml
- filename: google-ads-customers-api-openapi.yml
  format: yaml
  label: Google Ads Customers API
  slug: google-ads-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-customers-api-openapi.yml
- filename: google-ads-keywords-api-openapi.yml
  format: yaml
  label: Google Ads Keywords API
  slug: google-ads-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-keywords-api-openapi.yml
- filename: google-ads-reporting-api-openapi.yml
  format: yaml
  label: Google Ads Reporting API
  slug: google-ads-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-reporting-api-openapi.yml
- filename: google-ads-api-v25-openapi.yml
  format: yaml
  label: Google Ads API
  slug: google-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-api-v25-openapi.yml
auth_types:
- oauth2
description: Google Ads authentication is two credentials that are easy to confuse and independently sufficient to break a call. OAuth 2.0 identifies the USER and grants the single adwords scope. The developer token identifies the APPLICATION and gates what it may reach and how much of it. A correct OAuth token with a Test-access developer token cannot touch a production account, and no amount of re-authorising will fix it — that is an application to Google, not a token refresh.
kind: authentication
layout: security
method: searched
name: Google Ads Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Ads secures its APIs with oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Ads
provider_slug: google-ads
scheme_count: 4
schemes:
- description: Authorization code flow issued by Google's identity platform. Endpoints confirmed against the live OIDC discovery document at https://accounts.google.com/.well-known/openid-configuration.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    refreshUrl: https://oauth2.googleapis.com/token
    revocationUrl: https://oauth2.googleapis.com/revoke
    scope_list:
    - https://www.googleapis.com/auth/adwords
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - discovery/google-ads-api-v25-discovery.json
  - openapi/google-ads-api-v25-openapi.yml
  - well-known/google-ads-openid-configuration.json
  type: oauth2
- description: Issued per Google Ads manager account through the API Center. Carries an access level — Test, Explorer, Basic or Standard — that determines both which accounts may be called and the daily operation quota. See plans/ and rate-limits/.
  in: header
  name: developerToken
  parameter_name: developer-token
  required: true
  sources:
  - https://developers.google.com/google-ads/api/docs/access-levels
  type: apiKey
- description: Customer ID of the manager account making the call on behalf of a client account. Digits only, no hyphens. Omitting it when required produces USER_PERMISSION_DENIED even with a valid token.
  in: header
  name: loginCustomerId
  parameter_name: login-customer-id
  required: conditional
  type: apiKey
- description: Used by third-party app analytics providers uploading to an account they are linked to rather than managing.
  in: header
  name: linkedCustomerId
  parameter_name: linked-customer-id
  required: conditional
  type: apiKey
slug: google-ads-authentication
source_filename: google-ads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developers.google.com/google-ads/api/docs/oauth/overview,\n  https://developers.google.com/google-ads/api/docs/access-levels,\n  https://developers.google.com/google-ads/api/docs/concepts/call-structure,\n  well-known/google-ads-openid-configuration.json (live probe 2026-08-13) and\n  discovery/google-ads-api-v25-discovery.json\ndocs: https://developers.google.com/google-ads/api/docs/oauth/overview\nprovider: Google Ads\nproviderId: google-ads\ndescription: >-\n  Google Ads authentication is two credentials that are easy to confuse and independently\n  sufficient to break a call. OAuth 2.0 identifies the USER and grants the single adwords\n  scope. The developer token identifies the APPLICATION and gates what it may reach and\n  how much of it. A correct OAuth token with a Test-access developer token cannot touch a\n  production account, and no amount of re-authorising will fix it — that is an\n  application to\
  \ Google, not a token refresh.\nsummary:\n  types:\n    - oauth2\n  oauth2_flows:\n    - authorizationCode\n  additional_required_headers:\n    - developer-token\n  scope_count: 1\nschemes:\n  - name: oauth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n        refreshUrl: https://oauth2.googleapis.com/token\n        revocationUrl: https://oauth2.googleapis.com/revoke\n        scopes: 1\n        scope_list:\n          - https://www.googleapis.com/auth/adwords\n    description: >-\n      Authorization code flow issued by Google's identity platform. Endpoints confirmed\n      against the live OIDC discovery document at\n      https://accounts.google.com/.well-known/openid-configuration.\n    sources:\n      - discovery/google-ads-api-v25-discovery.json\n      - openapi/google-ads-api-v25-openapi.yml\n      - well-known/google-ads-openid-configuration.json\n\
  \  - name: developerToken\n    type: apiKey\n    in: header\n    parameter_name: developer-token\n    required: true\n    description: >-\n      Issued per Google Ads manager account through the API Center. Carries an access\n      level — Test, Explorer, Basic or Standard — that determines both which accounts may\n      be called and the daily operation quota. See plans/ and rate-limits/.\n    sources:\n      - https://developers.google.com/google-ads/api/docs/access-levels\n  - name: loginCustomerId\n    type: apiKey\n    in: header\n    parameter_name: login-customer-id\n    required: conditional\n    description: >-\n      Customer ID of the manager account making the call on behalf of a client account.\n      Digits only, no hyphens. Omitting it when required produces\n      USER_PERMISSION_DENIED even with a valid token.\n  - name: linkedCustomerId\n    type: apiKey\n    in: header\n    parameter_name: linked-customer-id\n    required: conditional\n    description: >-\n      Used\
  \ by third-party app analytics providers uploading to an account they are linked\n      to rather than managing.\ncredential_types:\n  - name: OAuth desktop / web client\n    note: Standard interactive user consent producing a refresh token stored by the app.\n  - name: Application Default Credentials\n    note: >-\n      gcloud auth application-default login --scopes\n      https://www.googleapis.com/auth/adwords — the path Google's own MCP server documents.\n  - name: Service account with domain-wide delegation\n    note: >-\n      Supported only for Google Workspace domains, impersonating a user who has Google Ads\n      access. A bare service account cannot access Google Ads accounts.\nservice_accounts:\n  supported: partial\n  note: >-\n    There is no service-account-only path to the Google Ads API. Machine-to-machine access\n    still resolves to a human Google Ads user, either through a stored refresh token or\n    through domain-wide delegation impersonation.\ntoken_lifetime:\n\
  \  access_token: 3600 seconds (1 hour)\n  refresh_token: >-\n    Long-lived; revoked on password change, explicit revocation, six months of disuse, or\n    when an unverified app in testing status expires its tokens after 7 days.\nmtls:\n  supported: false\nsecurity_notes:\n  - >-\n    The single adwords scope grants read, write and delete across every account the\n    authenticating user can reach. Scope-level least privilege is not available — see\n    scopes/google-ads-scopes.yml.\n  - >-\n    A developer token is a shared secret across every customer an application manages.\n    Leaking it is materially worse than leaking one user's refresh token.\n  - >-\n    Test accounts use the PRODUCTION manager account's developer token, so the same\n    secret spans both environments. See sandbox/google-ads-sandbox.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/authentication/google-ads-authentication.yml
summary_line: oauth2 · 4 schemes
tags:
- Advertising
- Campaign Management
- Digital Advertising
- Google
- Marketing
- PPC
---
