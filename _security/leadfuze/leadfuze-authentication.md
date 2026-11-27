---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: leadfuze-email-verification-api-openapi.yml
  format: yaml
  label: LeadFuze Email verification API
  slug: leadfuze-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-email-verification-api-openapi.yml
- filename: leadfuze-enrichment-api-openapi.yml
  format: yaml
  label: LeadFuze Enrichment API
  slug: leadfuze-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-enrichment-api-openapi.yml
- filename: leadfuze-identity-resolution-pixel-api-openapi.yml
  format: yaml
  label: LeadFuze Identity Resolution Pixel API
  slug: leadfuze-identity-resolution-pixel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-identity-resolution-pixel-api-openapi.yml
- filename: leadfuze-integrations-api-openapi.yml
  format: yaml
  label: LeadFuze Integrations API
  slug: leadfuze-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-integrations-api-openapi.yml
- filename: leadfuze-intent-data-api-openapi.yml
  format: yaml
  label: LeadFuze Intent data API
  slug: leadfuze-intent-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-intent-data-api-openapi.yml
- filename: leadfuze-lead-database-api-openapi.yml
  format: yaml
  label: LeadFuze Lead database API
  slug: leadfuze-lead-database-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-lead-database-api-openapi.yml
- filename: leadfuze-phone-validation-api-openapi.yml
  format: yaml
  label: LeadFuze Phone validation API
  slug: leadfuze-phone-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfuze/openapi/leadfuze-phone-validation-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: LeadFuze Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeadFuze secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LeadFuze
provider_slug: leadfuze
scheme_count: 2
schemes:
- description: 'Authorization: Bearer YOUR_API_KEY. Create keys in the LeadFuze app.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/leadfuze-openapi.json
  type: http
- description: For file downloads opened in a browser.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/leadfuze-openapi.json
  type: apiKey
slug: leadfuze-authentication
source_filename: leadfuze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/leadfuze-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer YOUR_API_KEY. Create keys in the LeadFuze app.'\n  sources:\n  - openapi/leadfuze-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: For file downloads opened in a browser.\n  sources:\n  - openapi/leadfuze-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/leadfuze/authentication/leadfuze-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Lead Generation
- Sales
- Marketing
- Data Enrichment
- B2B
---
