---
api_key_in: []
api_specs:
- filename: revcontent-access-api-openapi.yml
  format: yaml
  label: RevContent Access API
  slug: revcontent-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-access-api-openapi.yml
- filename: revcontent-ccpa-api-openapi.yml
  format: yaml
  label: RevContent CCPA API
  slug: revcontent-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-ccpa-api-openapi.yml
- filename: revcontent-content-api-openapi.yml
  format: yaml
  label: RevContent Content API
  slug: revcontent-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-content-api-openapi.yml
- filename: revcontent-conversions-api-openapi.yml
  format: yaml
  label: RevContent Conversions API
  slug: revcontent-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-conversions-api-openapi.yml
- filename: revcontent-helpers-api-openapi.yml
  format: yaml
  label: RevContent Helpers API
  slug: revcontent-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-helpers-api-openapi.yml
- filename: revcontent-sub-accounts-api-openapi.yml
  format: yaml
  label: RevContent Sub Accounts API
  slug: revcontent-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-sub-accounts-api-openapi.yml
- filename: revcontent-targeting-api-openapi.yml
  format: yaml
  label: RevContent Targeting API
  slug: revcontent-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-targeting-api-openapi.yml
- filename: revcontent-widget-internal-content-api-openapi.yml
  format: yaml
  label: RevContent Widget Internal Content API
  slug: revcontent-widget-internal-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-internal-content-api-openapi.yml
- filename: revcontent-widget-optimizer-api-openapi.yml
  format: yaml
  label: RevContent Widget Optimizer API
  slug: revcontent-widget-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-optimizer-api-openapi.yml
- filename: revcontent-campaigns-api-openapi.yml
  format: yaml
  label: RevContent Campaigns API
  slug: revcontent-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-campaigns-api-openapi.yml
- filename: revcontent-widget-api-openapi.yml
  format: yaml
  label: RevContent Widget API
  slug: revcontent-widget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-api-openapi.yml
auth_types:
- oauth2
- http
description: 'RevContent uses a single auth model across all 43 documented operations: an OAuth 2.0 client-credentials grant that yields a 24-hour bearer token. There are no scopes, no refresh token, no OIDC and no OAuth server metadata document.'
kind: authentication
layout: security
method: searched
name: Revcontent Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: RevContent secures its APIs with oauth2 and http across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: RevContent
provider_slug: revcontent
scheme_count: 1
schemes:
- applies_to: all 43 documented operations except POST /oauth/token itself
  description: 'OAuth 2.0 client-credentials access token obtained from POST /oauth/token. Valid for 24 hours. Sent as ''Authorization: Bearer {access token}'' alongside ''Content-type: application/json''.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/revcontent-access-api-openapi.yml
  - openapi/revcontent-boosts-api-openapi.yml
  - openapi/revcontent-ccpa-api-openapi.yml
  - openapi/revcontent-content-api-openapi.yml
  - openapi/revcontent-conversions-api-openapi.yml
  - openapi/revcontent-helpers-api-openapi.yml
  - openapi/revcontent-sub-accounts-api-openapi.yml
  - openapi/revcontent-targeting-api-openapi.yml
  - openapi/revcontent-widget-internal-content-api-openapi.yml
  - openapi/revcontent-widget-optimizer-api-openapi.yml
  - openapi/revcontent-widgets-api-openapi.yml
  type: http
slug: revcontent-authentication
source_filename: revcontent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/ (11 specs) + https://api.revcontent.io/docs/stats/api_data.json\ndocs: https://help.revcontent.com/knowledge/publisher-advertiser-api-requests\ndescription: >-\n  RevContent uses a single auth model across all 43 documented operations: an OAuth 2.0\n  client-credentials grant that yields a 24-hour bearer token. There are no scopes, no refresh\n  token, no OIDC and no OAuth server metadata document.\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  scopes: 2\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    OAuth 2.0 client-credentials access token obtained from POST /oauth/token. Valid for 24 hours.\n    Sent as 'Authorization: Bearer {access token}' alongside 'Content-type: application/json'.\n  applies_to: all 43 documented operations except POST /oauth/token itself\n  sources:\n  - openapi/revcontent-access-api-openapi.yml\n\
  \  - openapi/revcontent-boosts-api-openapi.yml\n  - openapi/revcontent-ccpa-api-openapi.yml\n  - openapi/revcontent-content-api-openapi.yml\n  - openapi/revcontent-conversions-api-openapi.yml\n  - openapi/revcontent-helpers-api-openapi.yml\n  - openapi/revcontent-sub-accounts-api-openapi.yml\n  - openapi/revcontent-targeting-api-openapi.yml\n  - openapi/revcontent-widget-internal-content-api-openapi.yml\n  - openapi/revcontent-widget-optimizer-api-openapi.yml\n  - openapi/revcontent-widgets-api-openapi.yml\ntoken_endpoint:\n  url: https://api.revcontent.io/oauth/token\n  method: POST\n  content_type: application/x-www-form-urlencoded\n  grant_type: client_credentials\n  parameters:\n    - grant_type\n    - client_id\n    - client_secret\n  response_field: access_token\n  response_shape: '{\"access_token\": \"...\", \"expires_in\": 86400, \"token_type\": \"Bearer\", \"scope\": \"advertiser publisher\"}'\n  ttl_seconds: 86400\n  refresh_token: false\n  operation: openapi/revcontent-access-api-openapi.yml#getOauthAccess\n\
  credentials:\n  location: Account Settings -> \"Stats API Credentials\"\n  fields: [client_id, client_secret]\n  provisioning: >-\n    NOT self-serve. API access must be enabled by a RevContent account representative before the\n    credentials section appears in Account Settings.\nauthorization_model:\n  scopes: [advertiser, publisher]\n  requestable: false\n  detail: >-\n    The issued token DOES carry scopes — RevContent's own published token example returns\n    \"scope\": \"advertiser publisher\" — but they are not requestable. There is no `scope` parameter on\n    the token request; the authorization server decides which of the two roles the credential pair\n    is entitled to and returns them. The effect is coarse role-based authorization, not\n    least-privilege: an account holding both roles gets one token that can do everything either role\n    can do, on every operation. See scopes/revcontent-scopes.yml.\n  multi_tenancy: >-\n    `sub_account_id` is a plain query/body parameter\
  \ on 18 operations, not a token boundary. A single\n    client-credentials token can act across every sub account reachable from the parent, so tenancy\n    is a caller convention rather than an enforced authorization scope.\ndiscovery:\n  openid_configuration: 404 on all hosts (2026-08-13)\n  oauth_authorization_server: 404 on all hosts (2026-08-13)\n  detail: >-\n    No RFC 8414 metadata and no OIDC discovery document, so the token endpoint cannot be discovered\n    programmatically — it is only documented in prose.\nexceptions:\n  - operation: postSubmitCCPARequest\n    detail: >-\n      POST /stats/api/v1.0/data_requests/submit is the one operation the provider documents without\n      a bearer token in its example. It is form-encoded and identifies the consumer through a\n      `Cookie: __ID=…` header, because it is issued from the consumer's browser context.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/authentication/revcontent-authentication.yml
summary_line: oauth2/http · 1 scheme
tags:
- Native Advertising
- Content Recommendation
- Ad Network
- Publisher Monetization
- Programmatic Advertising
- Advertising Technology
- Campaign Management
- Audience Targeting
- Conversion Tracking
- Marketing
---
