---
api_key_in:
- path
api_specs:
- filename: mixrank-account-api-openapi.yml
  format: yaml
  label: MixRank Account API
  slug: mixrank-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-account-api-openapi.yml
- filename: mixrank-audience-segments-api-openapi.yml
  format: yaml
  label: MixRank Audience Segments API
  slug: mixrank-audience-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-audience-segments-api-openapi.yml
- filename: mixrank-companies-api-openapi.yml
  format: yaml
  label: MixRank Companies API
  slug: mixrank-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-companies-api-openapi.yml
- filename: mixrank-email-api-openapi.yml
  format: yaml
  label: MixRank Email API
  slug: mixrank-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-email-api-openapi.yml
- filename: mixrank-ios-app-privacy-api-openapi.yml
  format: yaml
  label: MixRank iOS App Privacy API
  slug: mixrank-ios-app-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-app-privacy-api-openapi.yml
- filename: mixrank-ios-apps-api-openapi.yml
  format: yaml
  label: MixRank iOS Apps API
  slug: mixrank-ios-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-apps-api-openapi.yml
- filename: mixrank-ios-developers-api-openapi.yml
  format: yaml
  label: MixRank iOS Developers API
  slug: mixrank-ios-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-developers-api-openapi.yml
- filename: mixrank-ios-rankings-api-openapi.yml
  format: yaml
  label: MixRank iOS Rankings API
  slug: mixrank-ios-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-rankings-api-openapi.yml
- filename: mixrank-ios-sdks-api-openapi.yml
  format: yaml
  label: MixRank iOS SDKs API
  slug: mixrank-ios-sdks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-ios-sdks-api-openapi.yml
- filename: mixrank-people-api-openapi.yml
  format: yaml
  label: MixRank People API
  slug: mixrank-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-people-api-openapi.yml
- filename: mixrank-play-store-apps-api-openapi.yml
  format: yaml
  label: MixRank Play Store Apps API
  slug: mixrank-play-store-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-play-store-apps-api-openapi.yml
- filename: mixrank-play-store-developers-api-openapi.yml
  format: yaml
  label: MixRank Play Store Developers API
  slug: mixrank-play-store-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-play-store-developers-api-openapi.yml
- filename: mixrank-play-store-rankings-api-openapi.yml
  format: yaml
  label: MixRank Play Store Rankings API
  slug: mixrank-play-store-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-play-store-rankings-api-openapi.yml
- filename: mixrank-play-store-sdks-api-openapi.yml
  format: yaml
  label: MixRank Play Store SDKs API
  slug: mixrank-play-store-sdks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-play-store-sdks-api-openapi.yml
- filename: mixrank-web-tags-api-openapi.yml
  format: yaml
  label: MixRank Web Tags API
  slug: mixrank-web-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-web-tags-api-openapi.yml
- filename: mixrank-websites-api-openapi.yml
  format: yaml
  label: MixRank Websites API
  slug: mixrank-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/openapi/mixrank-websites-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mixrank Authentication
name_suffix: Authentication
oauth_flows: []
overview: MixRank secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MixRank
provider_slug: mixrank
scheme_count: 1
schemes:
- description: API key passed as a URL path segment. Not expressible as a standard OpenAPI apiKey securityScheme (which supports header/query/cookie only), so it is modeled as a server variable in openapi/mixrank-openapi.yml and documented here.
  in: path
  name: ApiKeyPath
  parameter: api_key
  sources:
  - https://mixrank.com/api/documentation
  type: apiKey
slug: mixrank-authentication
source_filename: mixrank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mixrank.com/api/documentation\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - path\n  oauth2_flows: []\n  notes: >-\n    MixRank authenticates every request with an API key supplied as a segment of\n    the request URL path (https://api.mixrank.com/v2/json/{api_key}/...), rather\n    than an Authorization header or query parameter. There is no OAuth surface.\n    An API key is obtained by logging in or requesting API access; the /echo\n    endpoint validates a key and /usage reports remaining quota.\nschemes:\n- name: ApiKeyPath\n  type: apiKey\n  in: path\n  parameter: api_key\n  description: >-\n    API key passed as a URL path segment. Not expressible as a standard OpenAPI\n    apiKey securityScheme (which supports header/query/cookie only), so it is\n    modeled as a server variable in openapi/mixrank-openapi.yml and documented\n    here.\n  sources:\n  - https://mixrank.com/api/documentation\nobtain:\n  url:\
  \ https://mixrank.com/login\n  request_access: https://mixrank.com/get-started/\nvalidate_operation: echo\nusage_operation: getUsage\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixrank/refs/heads/main/authentication/mixrank-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- Technographics
- Firmographics
- People Data
- Mobile Apps
- SDK Intelligence
- App Store
- Web Technology
- Sales Intelligence
- Data Enrichment
---
