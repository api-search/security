---
api_key_in:
- header
api_specs:
- filename: dow-jones-screening-and-monitoring-api-openapi.json
  format: json
  label: Dow Jones Screening and Monitoring API
  slug: screening-and-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-screening-and-monitoring-api-openapi.json
- filename: dow-jones-screening-and-monitoring-private-lists-api-openapi.json
  format: json
  label: Dow Jones Screening and Monitoring Private Lists API
  slug: screening-and-monitoring-private-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-screening-and-monitoring-private-lists-api-openapi.json
- filename: dow-jones-advanced-screening-and-monitoring-api-openapi.json
  format: json
  label: Dow Jones Advanced Screening and Monitoring API
  slug: advanced-screening-and-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-advanced-screening-and-monitoring-api-openapi.json
- filename: dow-jones-risk-search-api-openapi.json
  format: json
  label: Dow Jones Risk Search API
  slug: risk-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-risk-search-api-openapi.json
- filename: dow-jones-risk-profiles-api-openapi.json
  format: json
  label: Dow Jones Risk Profiles API
  slug: risk-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-risk-profiles-api-openapi.json
- filename: dow-jones-risk-taxonomy-api-openapi.json
  format: json
  label: Dow Jones Risk Taxonomy API
  slug: risk-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-risk-taxonomy-api-openapi.json
- filename: dow-jones-profile-version-history-api-openapi.json
  format: json
  label: Dow Jones Profile Version History API
  slug: profile-version-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-profile-version-history-api-openapi.json
- filename: dow-jones-due-diligence-reports-api-openapi.json
  format: json
  label: Dow Jones Due Diligence Reports API
  slug: due-diligence-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-due-diligence-reports-api-openapi.json
- filename: dow-jones-riskcenter-third-party-api-0-2-openapi.json
  format: json
  label: Dow Jones RiskCenter Third Party Platform API
  slug: riskcenter-third-party-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-riskcenter-third-party-api-0-2-openapi.json
- filename: dow-jones-newswires-real-time-api-openapi.json
  format: json
  label: Dow Jones Newswires Real-Time API
  slug: newswires-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-newswires-real-time-api-openapi.json
- filename: dow-jones-top-stories-api-openapi.json
  format: json
  label: Dow Jones Top Stories API
  slug: top-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-top-stories-api-openapi.json
- filename: dow-jones-calendar-live-api-openapi.json
  format: json
  label: Dow Jones Calendar Live API
  slug: calendar-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-calendar-live-api-openapi.json
- filename: dow-jones-newswires-content-api-openapi.json
  format: json
  label: Dow Jones Newswires Content API
  slug: newswires-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-newswires-content-api-openapi.json
- filename: dow-jones-content-api-swagger.json
  format: json
  label: Dow Jones Content API
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-content-api-swagger.json
- filename: dow-jones-newsletters-api-openapi.json
  format: json
  label: Dow Jones Factiva Newsletters API
  slug: newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-newsletters-api-openapi.json
- filename: dow-jones-company-news-radar-api-openapi.json
  format: json
  label: Dow Jones Company News Radar API
  slug: company-news-radar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/openapi/dow-jones-company-news-radar-api-openapi.json
auth_types:
- oauth2
- http bearer
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dow Jones Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password (service account)
- jwt-bearer
- refresh_token
overview: Dow Jones secures its APIs with oauth2, http bearer, and apiKey across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password (service account), jwt-bearer, and refresh_token flow(s).
provider_name: Dow Jones
provider_slug: dow-jones
scheme_count: 5
schemes:
- bearerFormat: JWT
  description: JWT authentication is the preferred authentication method, and should be used for new integrations.  Contact support to request a service account.
  name: jwt
  scheme: bearer
  sources:
  - openapi/dow-jones-advanced-screening-and-monitoring-api-openapi.json
  - openapi/dow-jones-calendar-live-api-openapi.json
  - openapi/dow-jones-company-news-radar-api-openapi.json
  - openapi/dow-jones-newsletters-api-openapi.json
  - openapi/dow-jones-newswires-content-api-openapi.json
  - openapi/dow-jones-newswires-real-time-api-openapi.json
  - openapi/dow-jones-profile-version-history-api-openapi.json
  - openapi/dow-jones-risk-profiles-api-openapi.json
  - openapi/dow-jones-risk-taxonomy-api-openapi.json
  - openapi/dow-jones-screening-and-monitoring-api-openapi.json
  - openapi/dow-jones-screening-and-monitoring-private-lists-api-openapi.json
  - openapi/dow-jones-top-stories-api-openapi.json
  type: http
- description: Basic authentication is supported for existing users, but is deprecated.  Existing users are encouraged to contact support for a dedicated service account and switch to JWT authentication.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/dow-jones-advanced-screening-and-monitoring-api-openapi.json
  type: http
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/dow-jones-content-api-swagger.json
  - openapi/dow-jones-due-diligence-reports-api-openapi.json
  - openapi/dow-jones-risk-search-api-openapi.json
  - openapi/dow-jones-riskcenter-third-party-api-0-1-openapi.json
  - openapi/dow-jones-riskcenter-third-party-api-0-2-openapi.json
  type: apiKey
- description: 'Factiva Integration API-key authentication: send the Dow Jones-issued user key in the user-key header.'
  docs: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication
  in: header
  name: user-key
  parameter: user-key
  sources:
  - docs
  type: apiKey
- authorizationUrl: https://sso.accounts.dowjones.com/authorize
  description: 'Dow Jones Identity Service: two-step token exchange. 1) POST /oauth2/v1/token (grant_type=password, connection=service-account, scope "openid service_account_id[ offline_access]") returns AuthN id_token+access_token; 2) POST /oauth2/v1/token (grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer, scope "openid pib") returns the AuthZ bearer JWT used on API calls (expires_in 36000). Authorization-code and implicit flows are available for user-facing apps; refresh_token renews AuthZ tokens.'
  docs: https://developer.dowjones.com/documents/site-docs-getting_started-sessions_and_authentication-dow_jones_identity_service
  name: dow-jones-identity-service
  scopes_artifact: scopes/dow-jones-scopes.yml
  sources:
  - docs
  tokenUrl: https://accounts.dowjones.com/oauth2/v1/token
  type: oauth2
slug: dow-jones-authentication
source_filename: dow-jones-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/dow-jones-advanced-screening-and-monitoring-api-openapi.json, openapi/dow-jones-calendar-live-api-openapi.json,\n  openapi/dow-jones-company-news-radar-api-openapi.json, openapi/dow-jones-content-api-swagger.json, openapi/dow-jones-due-diligence-reports-api-openapi.json,\n  openapi/dow-jones-newsletters-api-openapi.json, openapi/dow-jones-newswires-content-api-openapi.json, openapi/dow-jones-newswires-real-time-api-openapi.json,\n  openapi/dow-jones-profile-version-history-api-openapi.json, openapi/dow-jones-risk-profiles-api-openapi.json,\n  openapi/dow-jones-risk-search-api-openapi.json, openapi/dow-jones-risk-taxonomy-api-openapi.json ...\nsummary:\n  types:\n  - oauth2\n  - http bearer\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - password (service account)\n  - jwt-bearer\n  - refresh_token\n  identity_service: https://sso.accounts.dowjones.com/ (OIDC discovery\
  \ at accounts.dowjones.com/.well-known/openid-configuration)\nschemes:\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT authentication is the preferred authentication method, and should be used for new integrations.  Contact\n    support to request a service account.\n  sources:\n  - openapi/dow-jones-advanced-screening-and-monitoring-api-openapi.json\n  - openapi/dow-jones-calendar-live-api-openapi.json\n  - openapi/dow-jones-company-news-radar-api-openapi.json\n  - openapi/dow-jones-newsletters-api-openapi.json\n  - openapi/dow-jones-newswires-content-api-openapi.json\n  - openapi/dow-jones-newswires-real-time-api-openapi.json\n  - openapi/dow-jones-profile-version-history-api-openapi.json\n  - openapi/dow-jones-risk-profiles-api-openapi.json\n  - openapi/dow-jones-risk-taxonomy-api-openapi.json\n  - openapi/dow-jones-screening-and-monitoring-api-openapi.json\n  - openapi/dow-jones-screening-and-monitoring-private-lists-api-openapi.json\n  - openapi/dow-jones-top-stories-api-openapi.json\n\
  - name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication is supported for existing users, but is deprecated.  Existing users are encouraged\n    to contact support for a dedicated service account and switch to JWT authentication.\n  sources:\n  - openapi/dow-jones-advanced-screening-and-monitoring-api-openapi.json\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/dow-jones-content-api-swagger.json\n  - openapi/dow-jones-due-diligence-reports-api-openapi.json\n  - openapi/dow-jones-risk-search-api-openapi.json\n  - openapi/dow-jones-riskcenter-third-party-api-0-1-openapi.json\n  - openapi/dow-jones-riskcenter-third-party-api-0-2-openapi.json\n- name: user-key\n  type: apiKey\n  in: header\n  parameter: user-key\n  description: 'Factiva Integration API-key authentication: send the Dow Jones-issued user key in the user-key header.'\n  docs: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication\n\
  \  sources:\n  - docs\n- name: dow-jones-identity-service\n  type: oauth2\n  description: 'Dow Jones Identity Service: two-step token exchange. 1) POST /oauth2/v1/token (grant_type=password,\n    connection=service-account, scope \"openid service_account_id[ offline_access]\") returns AuthN id_token+access_token;\n    2) POST /oauth2/v1/token (grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer, scope \"openid pib\") returns\n    the AuthZ bearer JWT used on API calls (expires_in 36000). Authorization-code and implicit flows are available\n    for user-facing apps; refresh_token renews AuthZ tokens.'\n  tokenUrl: https://accounts.dowjones.com/oauth2/v1/token\n  authorizationUrl: https://sso.accounts.dowjones.com/authorize\n  docs: https://developer.dowjones.com/documents/site-docs-getting_started-sessions_and_authentication-dow_jones_identity_service\n  scopes_artifact: scopes/dow-jones-scopes.yml\n  sources:\n  - docs\ndocs: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dow-jones/refs/heads/main/authentication/dow-jones-authentication.yml
summary_line: oauth2/http bearer/apiKey · 5 schemes
tags:
- Financial
- Market Data
- News
- Publishing
- Risk and Compliance
- Screening
- Due Diligence
- Media Monitoring
---
