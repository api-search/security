---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: keysavvy-authentication-api-openapi.yml
  format: yaml
  label: KeySavvy Authentication API
  slug: keysavvy-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-authentication-api-openapi.yml
- filename: keysavvy-deal-documents-api-openapi.yml
  format: yaml
  label: KeySavvy Deal Documents API
  slug: keysavvy-deal-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-deal-documents-api-openapi.yml
- filename: keysavvy-deal-management-api-openapi.yml
  format: yaml
  label: KeySavvy Deal Management API
  slug: keysavvy-deal-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-deal-management-api-openapi.yml
- filename: keysavvy-documents-api-openapi.yml
  format: yaml
  label: KeySavvy Documents API
  slug: keysavvy-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-documents-api-openapi.yml
- filename: keysavvy-keysavvy-partner-api-api-openapi.yml
  format: yaml
  label: KeySavvy KeySavvy Partner API
  slug: keysavvy-keysavvy-partner-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-keysavvy-partner-api-api-openapi.yml
- filename: keysavvy-marketplace-management-api-openapi.yml
  format: yaml
  label: KeySavvy Marketplace Management API
  slug: keysavvy-marketplace-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-marketplace-management-api-openapi.yml
- filename: keysavvy-organization-management-api-openapi.yml
  format: yaml
  label: KeySavvy Organization Management API
  slug: keysavvy-organization-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-organization-management-api-openapi.yml
- filename: keysavvy-reporting-api-openapi.yml
  format: yaml
  label: KeySavvy Reporting API
  slug: keysavvy-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-reporting-api-openapi.yml
- filename: keysavvy-user-management-api-openapi.yml
  format: yaml
  label: KeySavvy User Management API
  slug: keysavvy-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-user-management-api-openapi.yml
- filename: keysavvy-vehicle-management-api-openapi.yml
  format: yaml
  label: KeySavvy Vehicle Management API
  slug: keysavvy-vehicle-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-vehicle-management-api-openapi.yml
- filename: keysavvy-webhook-management-api-openapi.yml
  format: yaml
  label: KeySavvy Webhook Management API
  slug: keysavvy-webhook-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keysavvy/openapi/keysavvy-webhook-management-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Keysavvy Authentication
name_suffix: Authentication
oauth_flows: []
overview: KeySavvy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KeySavvy
provider_slug: keysavvy
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: keysavvy-api
  sources:
  - openapi/keysavvy-openapi.json
  type: apiKey
slug: keysavvy-authentication
source_filename: keysavvy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: derived\nsource: openapi/keysavvy-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: keysavvy-api\n  sources:\n  - openapi/keysavvy-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/keysavvy/authentication/keysavvy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Automotive
- Marketplace
- API
- FinTech
---
