---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: foreign-agricultural-service-fas-open-data-swagger.json
  format: json
  label: USDA FAS Open Data API
  slug: fas-open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/_original/foreign-agricultural-service-fas-open-data-swagger.json
- filename: foreign-agricultural-service-esr-api-openapi.yml
  format: yaml
  label: Foreign Agricultural Service ESR API
  slug: foreign-agricultural-service-esr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/foreign-agricultural-service-esr-api-openapi.yml
- filename: foreign-agricultural-service-gats-api-openapi.yml
  format: yaml
  label: Foreign Agricultural Service GATS API
  slug: foreign-agricultural-service-gats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/foreign-agricultural-service-gats-api-openapi.yml
- filename: foreign-agricultural-service-psd-api-openapi.yml
  format: yaml
  label: Foreign Agricultural Service PSD API
  slug: foreign-agricultural-service-psd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/foreign-agricultural-service-psd-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Foreign Agricultural Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Foreign Agricultural Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Foreign Agricultural Service
provider_slug: foreign-agricultural-service
scheme_count: 1
schemes:
- applied: globally — the contract declares a root-level `security` requirement naming this scheme, and every one of the 35 operations inherits it
  description: API Key Authentication (verbatim from the contract's securityDefinitions)
  format: the raw key value, with no scheme prefix (not `Bearer`, not `ApiKey`)
  in: header
  name: apiKey
  parameter: API_KEY
  query_parameter_accepted: false
  query_parameter_note: 'The contract declares `in: header` only. Keeping the credential out of the URL is the safer of the two designs — it stays out of access logs, Referer headers and browser history — and it is worth crediting FAS for, because plenty of open-data APIs do the opposite.'
  sources:
  - openapi/_original/foreign-agricultural-service-fas-open-data-swagger.json
  - openapi/foreign-agricultural-service-esr-api-openapi.yml
  - openapi/foreign-agricultural-service-gats-api-openapi.yml
  - openapi/foreign-agricultural-service-psd-api-openapi.yml
  type: apiKey
slug: foreign-agricultural-service-authentication
source_filename: foreign-agricultural-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: >-\n  openapi/_original/foreign-agricultural-service-fas-open-data-swagger.json (the provider's\n  live Swagger 2.0 at https://apps.fas.usda.gov/opendata/swagger/docs/v1), the OpendataWeb\n  portal signup flow, and live probes on 2026-09-10\ndocs: https://apps.fas.usda.gov/opendatawebv2/#/signup\nnote: >-\n  Upgraded from derived to searched: the derived pass read the scheme out of the refined\n  OpenAPIs, this one adds the provider's own contract wording, the issuance flow read out of\n  the portal bundle, and the observed failure behaviour. FAS publishes no prose authentication\n  guide — the Swagger UI and the signup form are the whole of it.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  scopes: 0\n  scopes_note: >-\n    No OAuth, no scopes, no permissions model, so no scopes/ artifact is written. A key is\n    all-or-nothing across all 35 operations and all three datasets — there\
  \ is no way to issue\n    a key limited to, say, PSD.\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter: API_KEY\n    description: 'API Key Authentication (verbatim from the contract''s securityDefinitions)'\n    applied: >-\n      globally — the contract declares a root-level `security` requirement naming this scheme,\n      and every one of the 35 operations inherits it\n    format: the raw key value, with no scheme prefix (not `Bearer`, not `ApiKey`)\n    query_parameter_accepted: false\n    query_parameter_note: >-\n      The contract declares `in: header` only. Keeping the credential out of the URL is the\n      safer of the two designs — it stays out of access logs, Referer headers and browser\n      history — and it is worth crediting FAS for, because plenty of open-data APIs do the\n      opposite.\n    sources:\n      - openapi/_original/foreign-agricultural-service-fas-open-data-swagger.json\n      - openapi/foreign-agricultural-service-esr-api-openapi.yml\n\
  \      - openapi/foreign-agricultural-service-gats-api-openapi.yml\n      - openapi/foreign-agricultural-service-psd-api-openapi.yml\nissuance:\n  cost: free\n  onboarding: self-serve\n  signup_url: https://apps.fas.usda.gov/opendatawebv2/#/signup\n  issuer: api.data.gov\n  mechanism: >-\n    The FAS portal embeds the api.data.gov signup widget — the Angular bundle at\n    apps.fas.usda.gov/opendatawebV2/main.*.js loads\n    https://api.data.gov/static/javascripts/signup_embed.js — so the key is minted by\n    api.data.gov and delivered by email, then presented to the FAS API directly.\n  gateway_note: >-\n    Precise distinction, because it changes what a consumer should expect: api.data.gov\n    ISSUES the key but does NOT proxy this API. apps.fas.usda.gov validates the key itself,\n    its responses carry none of the api.data.gov gateway headers, and its error body is FAS's\n    own. So api.data.gov's published rate limits and X-RateLimit headers do not apply here.\n  approval: automatic\
  \ — no application, no review, no terms acceptance beyond the signup form\n  key_rotation:\n    documented: false\n    note: no rotation, revocation or expiry policy is published, and the portal exposes no key-management screen\nobserved_failure_modes:\n  probed: '2026-09-10'\n  probed_endpoint: https://apps.fas.usda.gov/OpenData/api/esr/regions\n  not_probed: >-\n    The authenticated success path was not exercised. API Evangelist holds no FAS API key and\n    does not obtain credentials for profiled providers.\n  modes:\n  - condition: no API_KEY header\n    status: 403\n    body: '\"Bad API Key\"'\n    note: bare JSON string, not an object — a client parsing it as JSON gets a string, not a dict\n  - condition: malformed API_KEY value\n    status: 500\n    body: '{\"message\":\"An error has occurred.\"}'\n    note: >-\n      A real defect. An invalid credential should be 401 or 403; returning 500 tells retry\n      libraries to treat a permanent auth failure as a transient server error\
  \ and retry it.\n      Full write-up in errors/foreign-agricultural-service-problem-types.yml.\ntransport:\n  https_only: true\n  hsts: 'max-age=31536000; includeSubdomains; preload (observed on API responses)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/authentication/foreign-agricultural-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agriculture
- Federal-Government
- Trade
- Open-Data
- Commodities
- Exports
- Government
---
