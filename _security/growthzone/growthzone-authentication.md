---
api_key_in:
- header
api_specs:
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Contacts API
  slug: growthzone-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Memberships API
  slug: growthzone-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Groups & Directory API
  slug: growthzone-groups-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Scheduled Billing API
  slug: growthzone-scheduled-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Certifications API
  slug: growthzone-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Events API
  slug: growthzone-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone OAuth / OpenID Connect (SSO) API
  slug: growthzone-oauth-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Growthzone Authentication
name_suffix: Authentication
oauth_flows: []
overview: GrowthZone secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GrowthZone
provider_slug: growthzone
scheme_count: 1
schemes:
- description: 'Server authentication. Send `Authorization: ApiKey {API_Key}` where the API Key is issued per application by GrowthZone WebSupport. OAuth 2.0 / OpenID Connect (authorize/token/userinfo at growthzoneapp.com) is used for user SSO flows.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/growthzone-openapi.yml
  type: apiKey
slug: growthzone-authentication
source_filename: growthzone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/growthzone-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Server authentication. Send `Authorization: ApiKey {API_Key}` where the API\n    Key is issued per application by GrowthZone WebSupport. OAuth 2.0 / OpenID Connect (authorize/token/userinfo\n    at growthzoneapp.com) is used for user SSO flows.'\n  sources:\n  - openapi/growthzone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/authentication/growthzone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Association Management
- AMS
- Membership Management
- Chambers of Commerce
- ChamberMaster
- Member Directory
- Events
- Billing
---
