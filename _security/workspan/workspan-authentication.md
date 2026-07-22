---
api_key_in:
- header
- query
api_specs:
- filename: workspan-authentication-openapi.yml
  format: yaml
  label: WorkSpan Authentication API
  slug: workspan-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-authentication-openapi.yml
- filename: workspan-co-sell-openapi.yml
  format: yaml
  label: WorkSpan Co-Sell API
  slug: workspan-co-sell-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-co-sell-openapi.yml
- filename: workspan-scim-openapi.yml
  format: yaml
  label: WorkSpan SCIM API
  slug: workspan-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-scim-openapi.yml
- filename: workspan-users-openapi.yml
  format: yaml
  label: WorkSpan Users API
  slug: workspan-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-users-openapi.yml
- filename: workspan-bulk-openapi.yml
  format: yaml
  label: WorkSpan Bulk API
  slug: workspan-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-bulk-openapi.yml
- filename: workspan-company-openapi.yml
  format: yaml
  label: WorkSpan Company API
  slug: workspan-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-company-openapi.yml
- filename: workspan-events-openapi.yml
  format: yaml
  label: WorkSpan Events API
  slug: workspan-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-events-openapi.yml
- filename: workspan-marketplace-openapi.yml
  format: yaml
  label: WorkSpan Marketplace API
  slug: workspan-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-marketplace-openapi.yml
- filename: workspan-object-openapi.yml
  format: yaml
  label: WorkSpan Object API
  slug: workspan-object-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-object-openapi.yml
- filename: workspan-partner-account-load-openapi.yml
  format: yaml
  label: WorkSpan Partner Account Load API
  slug: workspan-partner-account-load-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-partner-account-load-openapi.yml
- filename: workspan-report-openapi.yml
  format: yaml
  label: WorkSpan Report API
  slug: workspan-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-report-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Workspan Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: WorkSpan secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: WorkSpan
provider_slug: workspan
scheme_count: 3
schemes:
- description: Documented as "Implementation of OAuth 2.0 (RFC 6749) with Client Credentials Grant type". POST /token returns access_token (Bearer, expires_in 3600) + refresh_token; DELETE /token invalidates it. The x-ws-env header selects the sandbox environment.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-sandbox.workspan.com/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/workspan-authentication-openapi.yml
  - https://developer.workspan.com/api-details#api=authentication-api
  type: oauth2
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/workspan-authentication-openapi.yml
  - openapi/workspan-bulk-openapi.yml
  - openapi/workspan-co-sell-openapi.yml
  - openapi/workspan-company-openapi.yml
  - openapi/workspan-events-openapi.yml
  - openapi/workspan-marketplace-openapi.yml
  - openapi/workspan-object-openapi.yml
  - openapi/workspan-partner-account-load-openapi.yml
  - openapi/workspan-report-openapi.yml
  - openapi/workspan-scim-openapi.yml
  - openapi/workspan-users-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/workspan-authentication-openapi.yml
  - openapi/workspan-bulk-openapi.yml
  - openapi/workspan-co-sell-openapi.yml
  - openapi/workspan-company-openapi.yml
  - openapi/workspan-events-openapi.yml
  - openapi/workspan-marketplace-openapi.yml
  - openapi/workspan-object-openapi.yml
  - openapi/workspan-partner-account-load-openapi.yml
  - openapi/workspan-report-openapi.yml
  - openapi/workspan-scim-openapi.yml
  - openapi/workspan-users-openapi.yml
  type: apiKey
slug: workspan-authentication
source_filename: workspan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/workspan-authentication-openapi.yml, openapi/workspan-bulk-openapi.yml, openapi/workspan-co-sell-openapi.yml,\n  openapi/workspan-company-openapi.yml, openapi/workspan-events-openapi.yml, openapi/workspan-marketplace-openapi.yml,\n  openapi/workspan-object-openapi.yml, openapi/workspan-partner-account-load-openapi.yml, openapi/workspan-report-openapi.yml,\n  openapi/workspan-scim-openapi.yml, openapi/workspan-users-openapi.yml\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.workspan.com/oauth/token\n  description: Documented as \"Implementation of OAuth 2.0 (RFC 6749) with Client Credentials Grant type\". POST /token\n    returns access_token (Bearer, expires_in 3600) + refresh_token; DELETE /token invalidates it.\
  \ The x-ws-env header\n    selects the sandbox environment.\n  sources:\n  - openapi/workspan-authentication-openapi.yml\n  - https://developer.workspan.com/api-details#api=authentication-api\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/workspan-authentication-openapi.yml\n  - openapi/workspan-bulk-openapi.yml\n  - openapi/workspan-co-sell-openapi.yml\n  - openapi/workspan-company-openapi.yml\n  - openapi/workspan-events-openapi.yml\n  - openapi/workspan-marketplace-openapi.yml\n  - openapi/workspan-object-openapi.yml\n  - openapi/workspan-partner-account-load-openapi.yml\n  - openapi/workspan-report-openapi.yml\n  - openapi/workspan-scim-openapi.yml\n  - openapi/workspan-users-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/workspan-authentication-openapi.yml\n  - openapi/workspan-bulk-openapi.yml\n  - openapi/workspan-co-sell-openapi.yml\n  - openapi/workspan-company-openapi.yml\n\
  \  - openapi/workspan-events-openapi.yml\n  - openapi/workspan-marketplace-openapi.yml\n  - openapi/workspan-object-openapi.yml\n  - openapi/workspan-partner-account-load-openapi.yml\n  - openapi/workspan-report-openapi.yml\n  - openapi/workspan-scim-openapi.yml\n  - openapi/workspan-users-openapi.yml\ndocs: https://developer.workspan.com/api-details#api=authentication-api\nnote: All gateway calls additionally carry the Azure APIM subscription key (Ocp-Apim-Subscription-Key header or\n  subscription-key query parameter).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/authentication/workspan-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Co-Sell
- Partnerships
- Ecosystem
- Cloud Marketplaces
- Sales
- B2B
- SaaS
---
