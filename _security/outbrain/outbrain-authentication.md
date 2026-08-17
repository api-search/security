---
api_key_in:
- header
- query
api_specs:
- filename: outbrain-authentication-api-openapi.yml
  format: yaml
  label: Outbrain Authentication API
  slug: outbrain-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-authentication-api-openapi.yml
- filename: outbrain-budgets-api-openapi.yml
  format: yaml
  label: Outbrain Budgets API
  slug: outbrain-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-budgets-api-openapi.yml
- filename: outbrain-campaigns-api-openapi.yml
  format: yaml
  label: Outbrain Campaigns API
  slug: outbrain-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-campaigns-api-openapi.yml
- filename: outbrain-conversions-api-openapi.yml
  format: yaml
  label: Outbrain Conversions API
  slug: outbrain-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-conversions-api-openapi.yml
- filename: outbrain-events-api-openapi.yml
  format: yaml
  label: Outbrain Events API
  slug: outbrain-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-events-api-openapi.yml
- filename: outbrain-marketers-api-openapi.yml
  format: yaml
  label: Outbrain Marketers API
  slug: outbrain-marketers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-marketers-api-openapi.yml
- filename: outbrain-promotedlinks-api-openapi.yml
  format: yaml
  label: Outbrain PromotedLinks API
  slug: outbrain-promotedlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-promotedlinks-api-openapi.yml
- filename: outbrain-recommendations-api-openapi.yml
  format: yaml
  label: Outbrain Recommendations API
  slug: outbrain-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-recommendations-api-openapi.yml
- filename: outbrain-reporting-api-openapi.yml
  format: yaml
  label: Outbrain Reporting API
  slug: outbrain-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-reporting-api-openapi.yml
- filename: outbrain-targeting-api-openapi.yml
  format: yaml
  label: Outbrain Targeting API
  slug: outbrain-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-targeting-api-openapi.yml
- filename: outbrain-amplify-api-full-openapi.yml
  format: yaml
  label: Outbrain Amplify API
  slug: outbrain-amplify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-amplify-api-full-openapi.yml
- filename: outbrain-teads-report-api-openapi.yml
  format: yaml
  label: Teads Report API
  slug: outbrain-teads-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-teads-report-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Outbrain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Outbrain secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Outbrain
provider_slug: outbrain
scheme_count: 4
schemes:
- acquire:
  - GET /login with HTTP Basic credentials
  - https://my.outbrain.com/create-token (web form)
  acquire_rate_limit: 2 requests per hour per user on /login
  description: Token obtained from GET /login (HTTP Basic) or from https://my.outbrain.com/create-token. Valid for 30 days.
  docs: https://amplifyv01.docs.apiary.io/
  in: header
  name: OBTokenAuth
  parameter: OB-TOKEN-V1
  revocation: All tokens issued before an account password or email change are revoked. Issuing a new token does not invalidate existing ones.
  sources:
  - openapi/outbrain-amplify-api-full-openapi.yml
  - openapi/outbrain-authentication-api-openapi.yml
  - openapi/outbrain-budgets-api-openapi.yml
  - openapi/outbrain-campaigns-api-openapi.yml
  - openapi/outbrain-conversions-api-openapi.yml
  - openapi/outbrain-events-api-openapi.yml
  - openapi/outbrain-marketers-api-openapi.yml
  - openapi/outbrain-promotedlinks-api-openapi.yml
  - openapi/outbrain-recommendations-api-openapi.yml
  - openapi/outbrain-reporting-api-openapi.yml
  - openapi/outbrain-targeting-api-openapi.yml
  token_lifetime_days: 30
  type: apiKey
- description: HTTP Basic credentials used only on GET /login to obtain an OB-TOKEN-V1 token.
  name: BasicAuth
  scheme: basic
  scope: Used only on GET /login to mint an OB-TOKEN-V1 token; never sent on any other operation.
  sources:
  - openapi/outbrain-amplify-api-full-openapi.yml
  - openapi/outbrain-authentication-api-openapi.yml
  - openapi/outbrain-budgets-api-openapi.yml
  - openapi/outbrain-campaigns-api-openapi.yml
  - openapi/outbrain-conversions-api-openapi.yml
  - openapi/outbrain-events-api-openapi.yml
  - openapi/outbrain-marketers-api-openapi.yml
  - openapi/outbrain-promotedlinks-api-openapi.yml
  - openapi/outbrain-recommendations-api-openapi.yml
  - openapi/outbrain-reporting-api-openapi.yml
  - openapi/outbrain-targeting-api-openapi.yml
  type: http
- also_used_by: Teads Advertiser Conversion API (https://r.teads.tv) — see openapi/_original/outbrain-teads-conversion-api-openapi.yml
  api: Teads Report API
  description: Teads OAuth bearer token supplied in the Authorization header. Requires a Teads platform account with reporting rights.
  docs: https://teadsapi.docs.apiary.io/
  header: 'Authorization: Bearer {token}'
  name: BearerAuth
  requires: A Teads platform account with reporting rights.
  scheme: bearer
  sources:
  - openapi/outbrain-teads-report-api-openapi.yml
  type: http
- api: Outbrain Engage API
  description: Publisher installation key passed as a query parameter to the Engage recommendation endpoint on odb.outbrain.com.
  in: query
  name: PublisherKeyAuth
  parameter: publisherKey
  sources:
  - openapi/_original/outbrain-engage-api-openapi.yml
  type: apiKey
slug: outbrain-authentication
source_filename: outbrain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://amplifyv01.docs.apiary.io/ (Authentications section) and https://teadsapi.docs.apiary.io/ (Authentication\n  section), reconciled against the OpenAPI securitySchemes\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  note: The Amplify API does not use OAuth 2.0 — it issues an opaque proprietary token carried in a custom OB-TOKEN-V1\n    header. The Teads Report API uses an OAuth bearer token in a standard Authorization header, but Teads publishes\n    no authorization endpoint, token endpoint or scope vocabulary, so there is no OAuth scope surface to catalogue\n    for this provider.\nschemes:\n- name: OBTokenAuth\n  type: apiKey\n  in: header\n  parameter: OB-TOKEN-V1\n  description: Token obtained from GET /login (HTTP Basic) or from https://my.outbrain.com/create-token. Valid for\n    30 days.\n  sources:\n  - openapi/outbrain-amplify-api-full-openapi.yml\n  - openapi/outbrain-authentication-api-openapi.yml\n\
  \  - openapi/outbrain-budgets-api-openapi.yml\n  - openapi/outbrain-campaigns-api-openapi.yml\n  - openapi/outbrain-conversions-api-openapi.yml\n  - openapi/outbrain-events-api-openapi.yml\n  - openapi/outbrain-marketers-api-openapi.yml\n  - openapi/outbrain-promotedlinks-api-openapi.yml\n  - openapi/outbrain-recommendations-api-openapi.yml\n  - openapi/outbrain-reporting-api-openapi.yml\n  - openapi/outbrain-targeting-api-openapi.yml\n  token_lifetime_days: 30\n  acquire:\n  - GET /login with HTTP Basic credentials\n  - https://my.outbrain.com/create-token (web form)\n  acquire_rate_limit: 2 requests per hour per user on /login\n  revocation: All tokens issued before an account password or email change are revoked. Issuing a new token does\n    not invalidate existing ones.\n  docs: https://amplifyv01.docs.apiary.io/\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic credentials used only on GET /login to obtain an OB-TOKEN-V1 token.\n  sources:\n  - openapi/outbrain-amplify-api-full-openapi.yml\n\
  \  - openapi/outbrain-authentication-api-openapi.yml\n  - openapi/outbrain-budgets-api-openapi.yml\n  - openapi/outbrain-campaigns-api-openapi.yml\n  - openapi/outbrain-conversions-api-openapi.yml\n  - openapi/outbrain-events-api-openapi.yml\n  - openapi/outbrain-marketers-api-openapi.yml\n  - openapi/outbrain-promotedlinks-api-openapi.yml\n  - openapi/outbrain-recommendations-api-openapi.yml\n  - openapi/outbrain-reporting-api-openapi.yml\n  - openapi/outbrain-targeting-api-openapi.yml\n  scope: Used only on GET /login to mint an OB-TOKEN-V1 token; never sent on any other operation.\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Teads OAuth bearer token supplied in the Authorization header. Requires a Teads platform account\n    with reporting rights.\n  sources:\n  - openapi/outbrain-teads-report-api-openapi.yml\n  api: Teads Report API\n  header: 'Authorization: Bearer {token}'\n  requires: A Teads platform account with reporting rights.\n  docs: https://teadsapi.docs.apiary.io/\n\
  \  also_used_by: Teads Advertiser Conversion API (https://r.teads.tv) — see openapi/_original/outbrain-teads-conversion-api-openapi.yml\n- name: PublisherKeyAuth\n  type: apiKey\n  in: query\n  parameter: publisherKey\n  api: Outbrain Engage API\n  description: Publisher installation key passed as a query parameter to the Engage recommendation endpoint on odb.outbrain.com.\n  sources:\n  - openapi/_original/outbrain-engage-api-openapi.yml\ndocs:\n- https://amplifyv01.docs.apiary.io/\n- https://teadsapi.docs.apiary.io/\n- https://my.outbrain.com/create-token\naccess_gate:\n  url: https://www.outbrain.com/partner-api/\n  note: Amplify API credentials are issued only to approved partners; the API is not self-serve.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/authentication/outbrain-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Advertising
- Native Advertising
- Open Web
- CTV
- Connected TV
- Video Advertising
- Content Discovery
- Programmatic
- Performance Marketing
- AdTech
- Teads
---
