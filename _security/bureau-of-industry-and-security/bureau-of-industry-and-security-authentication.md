---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: bureau-of-industry-and-security-csl-apim-export.yaml
  format: yaml
  label: Consolidated Screening List (CSL) API
  slug: consolidated-screening-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/openapi/_original/bureau-of-industry-and-security-csl-apim-export.yaml
- filename: bureau-of-industry-and-security-search-api-openapi.yml
  format: yaml
  label: Bureau of Industry and Security Search API
  slug: bureau-of-industry-and-security-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/openapi/bureau-of-industry-and-security-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bureau Of Industry And Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Industry and Security secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bureau of Industry and Security
provider_slug: bureau-of-industry-and-security
scheme_count: 2
schemes:
- description: Subscription key issued by the International Trade Administration Data Services Platform, sent as a request header. This is the variant ITA's own 401 challenge names.
  in: header
  name: subscriptionKey
  parameter: subscription-key
  sources:
  - openapi/bureau-of-industry-and-security-search-api-openapi.yml
  - openapi/_original/bureau-of-industry-and-security-csl-apim-export.yaml
  type: apiKey
- description: The same subscription key sent as a query-string parameter. Declared by ITA's own OpenAPI export as `apiKeyQuery`. A key in a URL is logged by proxies, browsers and server access logs — prefer the header.
  in: query
  name: subscriptionKeyQuery
  parameter: subscription-key
  sources:
  - openapi/_original/bureau-of-industry-and-security-csl-apim-export.yaml
  type: apiKey
slug: bureau-of-industry-and-security-authentication
source_filename: bureau-of-industry-and-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://developer.trade.gov/developer/apis/consolidated-screening-list?api-version=2022-04-01-preview&export=true&format=openapi\n  (ITA API Management, anonymous, 2026-09-05) · live 401 challenge from\n  https://data.trade.gov/consolidated_screening_list/v1/search · https://developer.trade.gov/signup\ndocs: https://developer.trade.gov/api-details#api=consolidated-screening-list&operation=search\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n    - query\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: subscriptionKey\n    type: apiKey\n    in: header\n    parameter: subscription-key\n    description: >-\n      Subscription key issued by the International Trade Administration Data Services\n      Platform, sent as a request header. This is the variant ITA's own 401 challenge names.\n    sources:\n      - openapi/bureau-of-industry-and-security-search-api-openapi.yml\n\
  \      - openapi/_original/bureau-of-industry-and-security-csl-apim-export.yaml\n  - name: subscriptionKeyQuery\n    type: apiKey\n    in: query\n    parameter: subscription-key\n    description: >-\n      The same subscription key sent as a query-string parameter. Declared by ITA's own\n      OpenAPI export as `apiKeyQuery`. A key in a URL is logged by proxies, browsers and\n      server access logs — prefer the header.\n    sources:\n      - openapi/_original/bureau-of-industry-and-security-csl-apim-export.yaml\nchallenge:\n  status: 401\n  header: >-\n    WWW-Authenticate: AzureApiManagementKey\n    realm=\"https://mds-apimanager.azure-api.net/consolidated_screening_list\",\n    name=\"subscription-key\", type=\"header\"\n  body: '{ \"statusCode\": 401, \"message\": \"Access denied due to missing subscription key. Make sure to include subscription key when making requests to an API.\" }'\n  observed: '2026-09-05'\nonboarding:\n  sign_up: https://developer.trade.gov/signup\n  sign_in:\
  \ https://developer.trade.gov/signin\n  approval_required: false\n  cost: free\n  subscriptions_limit: 1\n  steps:\n    - Register an account on the ITA Data Services Platform.\n    - Subscribe to the \"Data Services Platform APIs\" product.\n    - Send the issued key as the `subscription-key` header on every request.\n  note: >-\n    Self-serve with no approval gate — verified from the product catalogue\n    (approvalRequired: false), not from marketing copy.\nunauthenticated_surface:\n  exists: true\n  note: >-\n    The full dataset is readable with no credential at\n    https://data.trade.gov/downloadable_consolidated_screening_list/v1/consolidated.{json,csv,tsv}\n    (HTTP 206 on a ranged request, 2026-09-05). Only the query API requires a key.\nscopes:\n  supported: false\n  note: >-\n    A subscription key carries no scopes, no audience and no expiry. There is nothing to\n    delegate and nothing to narrow, so scopes/ is deliberately absent from this repository\n    rather than written\
  \ empty.\nrotation:\n  documented: false\n  note: >-\n    Azure API Management issues a primary and secondary key per subscription, which makes\n    zero-downtime rotation possible, but ITA documents no rotation guidance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/authentication/bureau-of-industry-and-security-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Compliance
- Export Controls
- Federal-Government
- Industries
- National Security
- Screening Lists
- Security
---
