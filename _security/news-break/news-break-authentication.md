---
api_key_in:
- header
- query
api_specs:
- filename: news-break-account-billing-api-openapi.yml
  format: yaml
  label: News Break Account Billing API
  slug: news-break-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-account-billing-api-openapi.yml
- filename: news-break-ad-account-api-openapi.yml
  format: yaml
  label: News Break Ad Account API
  slug: news-break-ad-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-ad-account-api-openapi.yml
- filename: news-break-ad-api-openapi.yml
  format: yaml
  label: News Break Ad API
  slug: news-break-ad-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-ad-api-openapi.yml
- filename: news-break-ad-set-api-openapi.yml
  format: yaml
  label: News Break Ad Set API
  slug: news-break-ad-set-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-ad-set-api-openapi.yml
- filename: news-break-campaign-api-openapi.yml
  format: yaml
  label: News Break Campaign API
  slug: news-break-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-campaign-api-openapi.yml
- filename: news-break-event-management-api-openapi.yml
  format: yaml
  label: News Break Event Management API
  slug: news-break-event-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-event-management-api-openapi.yml
- filename: news-break-organization-api-openapi.yml
  format: yaml
  label: News Break Organization API
  slug: news-break-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-organization-api-openapi.yml
- filename: news-break-report-api-openapi.yml
  format: yaml
  label: News Break Report API
  slug: news-break-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-report-api-openapi.yml
- filename: news-break-reporting-api-openapi.yml
  format: yaml
  label: News Break Reporting API
  slug: news-break-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-reporting-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: News Break Authentication
name_suffix: Authentication
oauth_flows: []
overview: News Break secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: News Break
provider_slug: news-break
scheme_count: 2
schemes:
- api: NewsBreak Advertising API
  description: Authorized access token. Carries the permissions granted by the advertiser on the ad account.
  example_header: 'Access-Token: your_access_token'
  in: header
  issuance:
    action: Generate Token
    location: NewsBreak Ad Manager -> Resources -> API Access Tokens
    prerequisite: An ad account must already exist in the NewsBreak Ad Manager.
    self_service: true
  name: AccessToken
  parameter_name: Access-Token
  sources:
  - openapi/news-break-advertising-openapi.yml
  transport: HTTP request header
  type: apiKey
- api: NewsBreak MSP Monetization Reporting API
  caveat: Credential-in-URL. Query-string secrets leak into access logs, referrer headers and CDN caches; this is a weaker posture than the header-based Advertising API scheme.
  description: API token for an MSP organization, sent as the `token` query parameter alongside the `org_id` and `app_id` query parameters that scope the request.
  in: query
  name: ApiToken
  parameter_name: token
  sources:
  - openapi/news-break-monetization-reporting-openapi.yml
  transport: URL query string
  type: apiKey
slug: news-break-authentication
source_filename: news-break-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://advertising-api.newsbreak.com/hc/en-us/articles/43889846961037-API-Integration-Guide\ndocs: https://advertising-api.newsbreak.com/hc/en-us/articles/43889846961037-API-Integration-Guide\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n    - query\n  oauth2_flows: []\n  oidc: false\n  mutual_tls: false\n  note: >-\n    NewsBreak uses long-lived, self-service API keys only. There is no OAuth 2.0, no OpenID Connect,\n    no scope surface, no refresh flow and no documented token expiry or rotation policy. The\n    Advertising API sends the key in a custom `Access-Token` header; the MSP Monetization Reporting\n    API sends it as a `token` query parameter, which puts the credential in URLs, proxy logs and\n    browser history.\nschemes:\n  - name: AccessToken\n    type: apiKey\n    in: header\n    parameter_name: Access-Token\n    api: NewsBreak Advertising API\n    sources:\n      - openapi/news-break-advertising-openapi.yml\n\
  \    description: >-\n      Authorized access token. Carries the permissions granted by the advertiser on the ad account.\n    issuance:\n      self_service: true\n      location: NewsBreak Ad Manager -> Resources -> API Access Tokens\n      action: Generate Token\n      prerequisite: An ad account must already exist in the NewsBreak Ad Manager.\n    transport: HTTP request header\n    example_header: 'Access-Token: your_access_token'\n  - name: ApiToken\n    type: apiKey\n    in: query\n    parameter_name: token\n    api: NewsBreak MSP Monetization Reporting API\n    sources:\n      - openapi/news-break-monetization-reporting-openapi.yml\n    description: >-\n      API token for an MSP organization, sent as the `token` query parameter alongside the `org_id`\n      and `app_id` query parameters that scope the request.\n    transport: URL query string\n    caveat: >-\n      Credential-in-URL. Query-string secrets leak into access logs, referrer headers and CDN\n      caches; this is a weaker\
  \ posture than the header-based Advertising API scheme.\nauthorization:\n  model: role-based, granted per ad account by the advertiser\n  roles:\n    - name: ORG_ADMIN\n      scope: organization\n      description: >-\n        Organization administrator. Required to update account spending caps. getAdminOrgs returns\n        the organizations where the caller holds this role.\n    - name: ACC_ADMIN\n      scope: ad account\n      description: Ad account administrator.\n    - name: ACC_OPERATOR\n      scope: ad account\n      description: Ad account operator.\n    - name: ACC_VIEWER\n      scope: ad account\n      description: Ad account read-only viewer.\n  assignment_operations:\n    - openapi/news-break-advertising-openapi.yml#addAdAccountUser\n    - openapi/news-break-advertising-openapi.yml#deleteAdAccountUser\n  enforcement: >-\n    Authorization failures surface as return code 403 (Permission denied) inside an HTTP 200\n    response body. Missing credentials return 4031 (Not login);\
  \ a bad token returns 4033\n    (Invalid access token).\ngaps:\n  - No documented token lifetime, expiry or rotation policy.\n  - No OAuth 2.0 or OpenID Connect; therefore no delegated authorization and no scopes.\n  - No documented token revocation endpoint.\n  - No mTLS, no request signing, no proof-of-possession.\n  - The MSP Reporting API passes the secret in the query string rather than a header.\nsee_also:\n  - errors/news-break-problem-types.yml\n  - conventions/news-break-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/authentication/news-break-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Advertising
- AdTech
- News
- Media
- Local News
- Publishing
- Monetization
- Campaign Management
- Reporting
- Analytics
- Content
---
