---
api_key_in:
- header
- query
api_specs:
- filename: appsflyer-raw-data-pull-api-v2-token-openapi.yml
  format: yaml
  label: Pull API (Reporting Data)
  slug: pull-api-reporting-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-raw-data-pull-api-v2-token-openapi.yml
- filename: appsflyer-server-to-server-events-api-for-mobile-openapi.yml
  format: yaml
  label: Events APIs (Server-to-Server & Client-to-Server)
  slug: events-apis-server-to-server-client-to-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-server-to-server-events-api-for-mobile-openapi.yml
- filename: appsflyer-app-management-api-v20-openapi.yml
  format: yaml
  label: Management APIs
  slug: management-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-app-management-api-v20-openapi.yml
- filename: appsflyer-audience-external-api-openapi.yml
  format: yaml
  label: Audience APIs
  slug: audience-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-audience-external-api-openapi.yml
- filename: appsflyer-onelink-api-v20-openapi.yml
  format: yaml
  label: OneLink API
  slug: onelink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-onelink-api-v20-openapi.yml
- filename: appsflyer-skan-aggregated-performance-report-api-openapi.yml
  format: yaml
  label: SKAdNetwork (SKAN) APIs
  slug: skadnetwork-skan-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-skan-aggregated-performance-report-api-openapi.yml
- filename: appsflyer-opendsr-api-openapi.yml
  format: yaml
  label: OpenDSR API
  slug: opendsr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-opendsr-api-openapi.yml
- filename: appsflyer-click-signing-api-openapi.yml
  format: yaml
  label: Click Signing API (Protect360)
  slug: click-signing-api-protect360
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-click-signing-api-openapi.yml
- filename: appsflyer-roi360-net-revenue-api-v20-openapi.yml
  format: yaml
  label: ROI360 Net Revenue API
  slug: roi360-net-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/openapi/appsflyer-roi360-net-revenue-api-v20-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Appsflyer Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppsFlyer secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppsFlyer
provider_slug: appsflyer
scheme_count: 4
schemes:
- description: "**Important: API V2 Token Revocation**\n\nAll API V2 tokens generated before March 10, 2026, 19:00 UTC have been revoked. If your token was generated before this date, please regenerate it. [Learn how](https://support.appsflyer.com/hc/en-us/articles/360004562377-Managing-AppsFlyer-tokens).\n\nAuthorization HTTP header containing API V2 token (bearer token) is required.\n\n The admin [gets the V2 token i"
  name: Bearer-Authentication
  scheme: bearer
  sources:
  - openapi/appsflyer-additional-identifiers-api-openapi.yml
  - openapi/appsflyer-adrevenue-account-integrations-api-openapi.yml
  - openapi/appsflyer-aggregate-pull-api-v2-token-openapi.yml
  - openapi/appsflyer-app-list-api-openapi.yml
  - openapi/appsflyer-app-management-api-v20-openapi.yml
  - openapi/appsflyer-audience-external-api-openapi.yml
  - openapi/appsflyer-audience-import-api-openapi.yml
  - openapi/appsflyer-audit-public-api-openapi.yml
  - openapi/appsflyer-click-signing-api-openapi.yml
  - openapi/appsflyer-cohort-api-openapi.yml
  - openapi/appsflyer-incost-api-1-openapi.yml
  - openapi/appsflyer-master-api-openapi.yml
  - openapi/appsflyer-master-freshness-api-openapi.yml
  - openapi/appsflyer-opendsr-api-openapi.yml
  - openapi/appsflyer-partner-integration-settings-api-openapi.yml
  - openapi/appsflyer-push-api-configuration-api-openapi.yml
  - openapi/appsflyer-raw-data-pull-api-v2-token-openapi.yml
  - openapi/appsflyer-roi360-net-revenue-api-v20-openapi.yml
  - openapi/appsflyer-skan-aggregated-performance-report-api-openapi.yml
  - openapi/appsflyer-skan-aggregated-postback-by-arrival-date-api-openapi.yml
  - openapi/appsflyer-skan-cv-schema-api-for-ad-networks-2-openapi.yml
  - openapi/appsflyer-skan-cv-schema-api-for-advertisers-1-openapi.yml
  - openapi/appsflyer-test-console-api-openapi.yml
  - openapi/appsflyer-user-management-openapi.yml
  type: http
- description: 'Pull API token for authentication.

    [Get the API token in the Dashboard](https://support.appsflyer.com/hc/en-us/articles/360004562377)'
  in: query
  name: ApiKeyAuth
  parameter: api_token
  sources:
  - openapi/appsflyer-aggregate-pull-api-v1-token-openapi.yml
  - openapi/appsflyer-raw-data-pull-api-v1-token-openapi.yml
  type: apiKey
- description: 'To get the authentication key, in AppsFlyer dashboard go to: App Settings > Dev Key'
  in: header
  name: ApiKeyAuth
  parameter: authentication
  sources:
  - openapi/appsflyer-legacy-server-to-server-events-api-for-mobile-openapi.yml
  - openapi/appsflyer-server-to-server-events-api-for-mobile-openapi.yml
  type: apiKey
- description: 'OneLink REST API token for authentication.

    [Get the API token in the Dashboard](https://support.appsflyer.com/hc/en-us/articles/360001250345-OneLink-API)'
  in: header
  name: ApiKeyAuth
  parameter: authorization
  sources:
  - openapi/appsflyer-onelink-api-v20-openapi.yml
  - openapi/appsflyer-pcconsolectv-client-app-events-api-openapi.yml
  - openapi/appsflyer-pcconsolectv-events-api-openapi.yml
  - openapi/appsflyer-preload-c2s-measurement-api-openapi.yml
  - openapi/appsflyer-preload-measurement-api-1-openapi.yml
  type: apiKey
slug: appsflyer-authentication
source_filename: appsflyer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/appsflyer-additional-identifiers-api-openapi.yml, openapi/appsflyer-adrevenue-account-integrations-api-openapi.yml,\n  openapi/appsflyer-aggregate-pull-api-v1-token-openapi.yml, openapi/appsflyer-aggregate-pull-api-v2-token-openapi.yml,\n  openapi/appsflyer-app-list-api-openapi.yml, openapi/appsflyer-app-management-api-v20-openapi.yml,\n  openapi/appsflyer-audience-external-api-openapi.yml, openapi/appsflyer-audience-import-api-openapi.yml,\n  openapi/appsflyer-audit-public-api-openapi.yml, openapi/appsflyer-click-signing-api-openapi.yml,\n  openapi/appsflyer-cohort-api-openapi.yml, openapi/appsflyer-incost-api-1-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: Bearer-Authentication\n  type: http\n  scheme: bearer\n  description: |-\n    **Important: API V2 Token Revocation**\n\n    All API V2 tokens generated before March 10, 2026, 19:00 UTC have been\
  \ revoked. If your token was generated before this date, please regenerate it. [Learn how](https://support.appsflyer.com/hc/en-us/articles/360004562377-Managing-AppsFlyer-tokens).\n\n    Authorization HTTP header containing API V2 token (bearer token) is required.\n\n     The admin [gets the V2 token i\n  sources:\n  - openapi/appsflyer-additional-identifiers-api-openapi.yml\n  - openapi/appsflyer-adrevenue-account-integrations-api-openapi.yml\n  - openapi/appsflyer-aggregate-pull-api-v2-token-openapi.yml\n  - openapi/appsflyer-app-list-api-openapi.yml\n  - openapi/appsflyer-app-management-api-v20-openapi.yml\n  - openapi/appsflyer-audience-external-api-openapi.yml\n  - openapi/appsflyer-audience-import-api-openapi.yml\n  - openapi/appsflyer-audit-public-api-openapi.yml\n  - openapi/appsflyer-click-signing-api-openapi.yml\n  - openapi/appsflyer-cohort-api-openapi.yml\n  - openapi/appsflyer-incost-api-1-openapi.yml\n  - openapi/appsflyer-master-api-openapi.yml\n  - openapi/appsflyer-master-freshness-api-openapi.yml\n\
  \  - openapi/appsflyer-opendsr-api-openapi.yml\n  - openapi/appsflyer-partner-integration-settings-api-openapi.yml\n  - openapi/appsflyer-push-api-configuration-api-openapi.yml\n  - openapi/appsflyer-raw-data-pull-api-v2-token-openapi.yml\n  - openapi/appsflyer-roi360-net-revenue-api-v20-openapi.yml\n  - openapi/appsflyer-skan-aggregated-performance-report-api-openapi.yml\n  - openapi/appsflyer-skan-aggregated-postback-by-arrival-date-api-openapi.yml\n  - openapi/appsflyer-skan-cv-schema-api-for-ad-networks-2-openapi.yml\n  - openapi/appsflyer-skan-cv-schema-api-for-advertisers-1-openapi.yml\n  - openapi/appsflyer-test-console-api-openapi.yml\n  - openapi/appsflyer-user-management-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_token\n  description: |-\n    Pull API token for authentication.\n    [Get the API token in the Dashboard](https://support.appsflyer.com/hc/en-us/articles/360004562377)\n  sources:\n  - openapi/appsflyer-aggregate-pull-api-v1-token-openapi.yml\n\
  \  - openapi/appsflyer-raw-data-pull-api-v1-token-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: authentication\n  description: 'To get the authentication key, in AppsFlyer dashboard go to: App Settings >\n    Dev Key'\n  sources:\n  - openapi/appsflyer-legacy-server-to-server-events-api-for-mobile-openapi.yml\n  - openapi/appsflyer-server-to-server-events-api-for-mobile-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: |-\n    OneLink REST API token for authentication.\n    [Get the API token in the Dashboard](https://support.appsflyer.com/hc/en-us/articles/360001250345-OneLink-API)\n  sources:\n  - openapi/appsflyer-onelink-api-v20-openapi.yml\n  - openapi/appsflyer-pcconsolectv-client-app-events-api-openapi.yml\n  - openapi/appsflyer-pcconsolectv-events-api-openapi.yml\n  - openapi/appsflyer-preload-c2s-measurement-api-openapi.yml\n  - openapi/appsflyer-preload-measurement-api-1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsflyer/refs/heads/main/authentication/appsflyer-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Mobile Attribution
- Marketing Analytics
- Mobile Measurement
- Deep Linking
- Audiences
- Ad Fraud Prevention
- SKAdNetwork
- Privacy
- Advertising Technology
- Mobile SDK
- Agentic AI
---
