---
api_key_in:
- query
api_specs:
- filename: google-pagespeed-analysis-api-openapi.yml
  format: yaml
  label: Google PageSpeed Analysis API
  slug: google-pagespeed-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pagespeed/refs/heads/main/openapi/google-pagespeed-analysis-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Pagespeed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google PageSpeed secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Google PageSpeed
provider_slug: google-pagespeed
scheme_count: 2
schemes:
- docs_statement: '"The API can be used with or without an API key, although a key is recommended for frequent, automated queries." ... "After you have an API key, your application can append the query parameter key=yourAPIKey to all request URLs. The API key is safe for embedding in URLs; it doesn''t need any encoding."'
  in: query
  key_issuance: https://console.cloud.google.com/apis/credentials
  key_restrictions: Cloud Console API keys can be restricted by referrer/IP and by API; a key restricted away from pagespeedonline.googleapis.com returns 400 API_KEY_INVALID.
  name: apiKey
  parameter: key
  probed_reality: Documented as optional, effectively mandatory. An unkeyed GET to https://www.googleapis.com/pagespeedonline/v5/runPagespeed on 2026-08-13 returned HTTP 429 RESOURCE_EXHAUSTED with quota_limit_value "0" — the shared anonymous pool is exhausted. Agents must treat the key as required.
  required: recommended
  sources:
  - openapi/google-pagespeed-analysis-api-openapi.yml
  - https://developers.google.com/speed/docs/insights/v5/get-started#APIKey
  type: apiKey
- alternative_parameter: access_token (query)
  in: header
  name: oauth2
  note: Declared in Google's Discovery document with the single identity scope `openid`. It is not the documented path for this API and grants no additional data access; see scopes/google-pagespeed-scopes.yml.
  parameter: Authorization
  scheme: bearer
  scopes:
  - openid
  sources:
  - https://pagespeedonline.googleapis.com/$discovery/rest?version=v5
  type: oauth2
slug: google-pagespeed-authentication
source_filename: google-pagespeed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/google-pagespeed-analysis-api-openapi.yml\ndocs: https://developers.google.com/speed/docs/insights/v5/get-started#APIKey\ndiscovery: https://pagespeedonline.googleapis.com/$discovery/rest?version=v5\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows: []\n  primary: apiKey\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  required: recommended\n  sources:\n  - openapi/google-pagespeed-analysis-api-openapi.yml\n  - https://developers.google.com/speed/docs/insights/v5/get-started#APIKey\n  docs_statement: >-\n    \"The API can be used with or without an API key, although a key is recommended for\n    frequent, automated queries.\" ... \"After you have an API key, your application can\n    append the query parameter key=yourAPIKey to all request URLs. The API key is safe\n    for embedding in URLs; it doesn't need any encoding.\"\n  probed_reality: >-\n    Documented\
  \ as optional, effectively mandatory. An unkeyed GET to\n    https://www.googleapis.com/pagespeedonline/v5/runPagespeed on 2026-08-13 returned\n    HTTP 429 RESOURCE_EXHAUSTED with quota_limit_value \"0\" — the shared anonymous pool is\n    exhausted. Agents must treat the key as required.\n  key_issuance: https://console.cloud.google.com/apis/credentials\n  key_restrictions: >-\n    Cloud Console API keys can be restricted by referrer/IP and by API; a key restricted\n    away from pagespeedonline.googleapis.com returns 400 API_KEY_INVALID.\n- name: oauth2\n  type: oauth2\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  alternative_parameter: access_token (query)\n  scopes: [openid]\n  sources:\n  - https://pagespeedonline.googleapis.com/$discovery/rest?version=v5\n  note: >-\n    Declared in Google's Discovery document with the single identity scope `openid`. It\n    is not the documented path for this API and grants no additional data access; see\n    scopes/google-pagespeed-scopes.yml.\n\
  transport_security:\n  https_required: true\n  tls_version_observed: TLSv1.3\nfailure_modes:\n  - {status: 400, reason: API_KEY_INVALID, meaning: key missing from the project, malformed, or restricted}\n  - {status: 429, reason: RATE_LIMIT_EXCEEDED, meaning: project or anonymous quota exhausted}\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pagespeed/refs/heads/main/authentication/google-pagespeed-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Core Web Vitals
- Google
- Lighthouse
- Page Speed
- SEO
- Web Performance
---
