---
api_key_in:
- header
api_specs:
- filename: groundtruth-ads-manager-openapi.yml
  format: yaml
  label: GroundTruth Ads Manager Public API
  slug: groundtruth-ads-manager-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groundtruth/refs/heads/main/openapi/groundtruth-ads-manager-openapi.yml
- filename: groundtruth-reporting-openapi.yml
  format: yaml
  label: Groundtruth Reporting API
  slug: groundtruth-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groundtruth/refs/heads/main/openapi/groundtruth-reporting-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Groundtruth Authentication
name_suffix: Authentication
oauth_flows: []
overview: GroundTruth secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GroundTruth
provider_slug: groundtruth
scheme_count: 2
schemes:
- description: Secret API key issued by GroundTruth on request.
  in: header
  name: api-key
  parameter: X-GT-API-KEY
  sources:
  - openapi/groundtruth-ads-manager-openapi.yml
  - openapi/groundtruth-reporting-openapi.yml
  type: apiKey
- description: Identifier of the user the key is issued to; sent alongside X-GT-API-KEY.
  in: header
  name: user-id
  parameter: X-GT-USER-ID
  sources:
  - openapi/groundtruth-ads-manager-openapi.yml
  - openapi/groundtruth-reporting-openapi.yml
  type: apiKey
slug: groundtruth-authentication
source_filename: groundtruth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/groundtruth-ads-manager-openapi.yml + openapi/groundtruth-reporting-openapi.yml\ndocs: https://api-docs.groundtruth.com/welcome-824669m0\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: >-\n    Paired-header API key. Both GroundTruth API surfaces require the SAME two headers together —\n    X-GT-USER-ID (the calling user's identifier) and X-GT-API-KEY (the secret). Neither header is\n    sufficient on its own. There is no OAuth 2.0, OIDC, mutual TLS or bearer-token flow on either\n    surface, and therefore no scope surface (scopes/ is intentionally absent).\n  credential_issuance: >-\n    Not self-serve. The provider's own reference states \"API credentials are provided on a request\n    basis\", and the help centre directs reporting-API users to contact support to request\n    credentials. There is no signup, key-provisioning or key-rotation endpoint in either spec.\nschemes:\n- name: api-key\n\
  \  type: apiKey\n  in: header\n  parameter: X-GT-API-KEY\n  description: Secret API key issued by GroundTruth on request.\n  sources:\n  - openapi/groundtruth-ads-manager-openapi.yml\n  - openapi/groundtruth-reporting-openapi.yml\n- name: user-id\n  type: apiKey\n  in: header\n  parameter: X-GT-USER-ID\n  description: Identifier of the user the key is issued to; sent alongside X-GT-API-KEY.\n  sources:\n  - openapi/groundtruth-ads-manager-openapi.yml\n  - openapi/groundtruth-reporting-openapi.yml\ndeclared_but_undefined:\n- name: session\n  used_by_operations: 248\n  note: >-\n    248 of the 259 Ads Manager operations list `session` in their `security` requirement, but\n    `session` is NOT defined in components.securitySchemes (only `api-key` and `user-id` are).\n    This is a real defect in the published contract: a generated client cannot resolve the scheme.\n    It most likely refers to the browser session cookie the ads.groundtruth.com console uses.\n    Recorded as observed; not\
  \ resolved, and not invented.\nobserved:\n- probe: GET https://api-public.groundtruth.com/accounts?tenant_id=1&organization_id=1\n  http_status: 401\n  body: '{\"errors\":[{\"code\":\"UNAUTHENTICATED\",\"message\":\"Sorry, you need to be authenticated to perform this operation.\"}]}'\n  fetched: '2026-08-12'\n- probe: GET https://reporting.groundtruth.com/demand/v1/campaign/1/daily\n  http_status: 401\n  header: 'x-amzn-ErrorType: UnauthorizedException'\n  fetched: '2026-08-12'\nunauthenticated_operations:\n  count: 11\n  note: >-\n    11 Ads Manager operations carry no `security` block at all (including GET /health and\n    GET /version). GET https://api-public.groundtruth.com/health returned 200 \"ok\" anonymously.\ncross_links:\n  conventions: conventions/groundtruth-conventions.yml\n  errors: errors/groundtruth-problem-types.yml\n  conformance: conformance/groundtruth-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groundtruth/refs/heads/main/authentication/groundtruth-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Martech
- Advertising
- Location Intelligence
- Marketing
- Adtech
- Location-Based Marketing
- Advertising API
- Campaign Management
- Ad Reporting
- Attribution
- Geofencing
- Digital Out Of Home
- CTV
---
