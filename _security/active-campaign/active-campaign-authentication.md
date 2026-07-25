---
api_key_in:
- header
api_specs:
- filename: activecampaign-api-v3
  format: yaml
  label: ActiveCampaign API v3
  slug: api-v3
  spec_type: Postman
  url: https://www.postman.com/acdevrel/activecampaign-developer-relations/collection/ju5a59q/activecampaign-api-v3
- filename: active-campaign-broadcasts-api-openapi.yml
  format: yaml
  label: ActiveCampaign Broadcasts API
  slug: active-campaign-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-broadcasts-api-openapi.yml
- filename: active-campaign-bulk-api-openapi.yml
  format: yaml
  label: ActiveCampaign Bulk API
  slug: active-campaign-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-bulk-api-openapi.yml
- filename: active-campaign-campaigns-api-openapi.yml
  format: yaml
  label: ActiveCampaign Campaigns API
  slug: active-campaign-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-campaigns-api-openapi.yml
- filename: active-campaign-contacts-api-openapi.yml
  format: yaml
  label: ActiveCampaign Contacts API
  slug: active-campaign-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-contacts-api-openapi.yml
- filename: active-campaign-custom-fields-api-openapi.yml
  format: yaml
  label: ActiveCampaign Custom Fields API
  slug: active-campaign-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-custom-fields-api-openapi.yml
- filename: active-campaign-deals-api-openapi.yml
  format: yaml
  label: ActiveCampaign Deals API
  slug: active-campaign-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-deals-api-openapi.yml
- filename: active-campaign-lists-api-openapi.yml
  format: yaml
  label: ActiveCampaign Lists API
  slug: active-campaign-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-lists-api-openapi.yml
- filename: active-campaign-segments-api-openapi.yml
  format: yaml
  label: ActiveCampaign Segments API
  slug: active-campaign-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-segments-api-openapi.yml
- filename: active-campaign-variables-api-openapi.yml
  format: yaml
  label: ActiveCampaign Variables API
  slug: active-campaign-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/openapi/active-campaign-variables-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Active Campaign Authentication
name_suffix: Authentication
oauth_flows: []
overview: ActiveCampaign secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ActiveCampaign
provider_slug: active-campaign
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Api-Token
  sources:
  - openapi/active-campaign-openapi.yml
  type: apiKey
slug: active-campaign-authentication
source_filename: active-campaign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/active-campaign-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Token\n  sources:\n  - openapi/active-campaign-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-campaign/refs/heads/main/authentication/active-campaign-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketing Automation
- Email Marketing
- CRM
- Customer Experience Automation
- Sales Engagement
---
