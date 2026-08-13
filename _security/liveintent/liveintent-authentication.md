---
api_key_in:
- header
api_specs:
- filename: liveintent-audiences-openapi.yml
  format: yaml
  label: LiveIntent Audiences API
  slug: audiences
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveintent/refs/heads/main/openapi/liveintent-audiences-openapi.yml
- filename: liveintent-privacy-openapi.yml
  format: yaml
  label: LiveIntent Privacy Management API
  slug: privacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveintent/refs/heads/main/openapi/liveintent-privacy-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Liveintent Authentication
name_suffix: Authentication
oauth_flows: []
overview: LiveIntent secures its APIs with apiKey and http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LiveIntent
provider_slug: liveintent
scheme_count: 1
schemes:
- description: For accessing internal endpoints an access token is required. It needs to be sent as a Bearer token in the Authorization header.
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/liveintent-audiences-openapi.yml
  - openapi/liveintent-privacy-openapi.yml
  type: apiKey
slug: liveintent-authentication
source_filename: liveintent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  openapi/liveintent-audiences-openapi.yml,\n  openapi/liveintent-privacy-openapi.yml, plus the provider auth documentation\n  listed under docs[] below.\ndocs:\n- https://audiences.liveintent.com/api-guide\n- https://privacy.liadm.com/api-guide\n- https://support.liveintent.com/connecting-to-liveintents-reporting-api/\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    All three documented LiveIntent APIs authenticate with an opaque bearer\n    token in the Authorization header. Two of them declare it in OpenAPI as an\n    apiKey scheme named \"Bearer\" in the header rather than as http/bearer, which\n    is why derive-authentication.py reports type apiKey. There is no OAuth 2.0\n    authorization server, no scopes, no OIDC discovery document and no\n    /.well-known/oauth-authorization-server on any LiveIntent host (all probed\n    404 or 401 on 2026-08-12), so scopes/ is intentionally\
  \ not emitted.\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    For accessing internal endpoints an access token is required. It needs to be\n    sent as a Bearer token in the Authorization header.\n  sources:\n  - openapi/liveintent-audiences-openapi.yml\n  - openapi/liveintent-privacy-openapi.yml\napis:\n- api: Audiences API\n  scheme: Bearer\n  location: header\n  header: 'Authorization: Bearer {token}'\n  token_issuance: >-\n    Not documented publicly. The API guide states only that an access token is\n    required; issuance is handled by the LiveIntent account team.\n  spec: openapi/liveintent-audiences-openapi.yml\n  observed:\n    url: https://audiences.liveintent.com/audiences\n    http_status: 401\n    body: '{\"errors\":[{\"httpStatus\":401,\"message\":\"Token not provided\",\"errorCode\":\"unauthorized\"}]}'\n    fetched: '2026-08-12'\n- api: Privacy Management API\n  scheme: Bearer\n  location: header\n  header: 'Authorization:\
  \ Bearer {token}'\n  token_issuance: >-\n    \"To get an access token, contact your account team at LiveIntent. Then use\n    the provided access token as a bearer token in the Authorization header\"\n    (privacy.liadm.com/api-guide, Authentication section). Tokens are issued by\n    a human, not by a token endpoint.\n  spec: openapi/liveintent-privacy-openapi.yml\n  authorization_model: >-\n    Account-category scoped rather than scope-scoped. A caller acts as a Media\n    Group (blanket over all child Publishers and Advertisers), a Publisher\n    (its publisherId plus related advertiserIds), an Advertiser (its\n    advertiserId only), or Global (authorized third-party agents submitting\n    industry-wide requests). The token carries the category; there is no\n    scope string.\n- api: Reporting API\n  scheme: http-bearer\n  location: header\n  header: 'Authorization: Bearer {token}'\n  token_endpoint: https://connect.liveintent.com/auth/login/\n  token_request: >-\n    POST /auth/login/\
  \ with application/json body {\"username\": \"...\",\n    \"password\": \"...\"} — a LiveIntent platform username and password pair.\n  token_response_fields: [token, username, userID, refreshToken]\n  token_lifetime: 12 hours\n  refresh: >-\n    A refreshToken is returned alongside the access token; the docs describe the\n    access token as revoked after 12 hours.\n  docs: https://support.liveintent.com/connecting-to-liveintents-reporting-api/\n  note: >-\n    LiveIntent's knowledge base calls this \"OAuth2\", but the documented flow is a\n    username/password login endpoint returning a bearer token — it is a\n    resource-owner-password-style login, not an RFC 6749 authorization server.\n    No authorize endpoint, no client_id, no scopes, and no discovery document\n    are published. Recorded here as observed rather than as the docs label it.\n  observed:\n    url: https://connect.liveintent.com/reporting/api/executeQuery\n    http_status: 401\n    body: Unauthorized\n    fetched:\
  \ '2026-08-12'\n- api: Programmatic Bidding API\n  scheme: none\n  note: >-\n    Server-to-server OpenRTB 2.5. LiveIntent is the exchange and sends bid\n    requests to a DSP-supplied bidding URL; the DSP does not authenticate to a\n    LiveIntent endpoint, so there is no client credential on this surface.\n  docs: https://support.liveintent.com/programmatic-bidding-api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveintent/refs/heads/main/authentication/liveintent-authentication.yml
summary_line: apiKey/http · 1 scheme
tags:
- Company
- Advertising
- AdTech
- Identity
- Email Marketing
- Audience
- Publishers
- Marketers
- Data
---
