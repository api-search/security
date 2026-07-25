---
api_key_in: []
api_specs:
- filename: ribbon-health-cost-estimates-api-openapi.yml
  format: yaml
  label: Ribbon Health Cost Estimates API
  slug: ribbon-health-cost-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-cost-estimates-api-openapi.yml
- filename: ribbon-health-filters-api-openapi.yml
  format: yaml
  label: Ribbon Health Filters API
  slug: ribbon-health-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-filters-api-openapi.yml
- filename: ribbon-health-focus-area-endpoints-api-openapi.yml
  format: yaml
  label: Ribbon Health Focus Area Endpoints API
  slug: ribbon-health-focus-area-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-focus-area-endpoints-api-openapi.yml
- filename: ribbon-health-locations-api-openapi.yml
  format: yaml
  label: Ribbon Health Locations API
  slug: ribbon-health-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-locations-api-openapi.yml
- filename: ribbon-health-networks-api-openapi.yml
  format: yaml
  label: Ribbon Health Networks API
  slug: ribbon-health-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-networks-api-openapi.yml
- filename: ribbon-health-organizations-api-openapi.yml
  format: yaml
  label: Ribbon Health Organizations API
  slug: ribbon-health-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-organizations-api-openapi.yml
- filename: ribbon-health-price-transparency-api-openapi.yml
  format: yaml
  label: Ribbon Health Price Transparency API
  slug: ribbon-health-price-transparency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-price-transparency-api-openapi.yml
- filename: ribbon-health-providers-api-openapi.yml
  format: yaml
  label: Ribbon Health Providers API
  slug: ribbon-health-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-providers-api-openapi.yml
- filename: ribbon-health-reference-endpoints-api-openapi.yml
  format: yaml
  label: Ribbon Health Reference Endpoints API
  slug: ribbon-health-reference-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-reference-endpoints-api-openapi.yml
- filename: ribbon-health-tins-api-openapi.yml
  format: yaml
  label: Ribbon Health TINs API
  slug: ribbon-health-tins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-tins-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ribbon Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ribbon Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ribbon Health
provider_slug: ribbon-health
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ribbon-health-h1-api-openapi.yml
  type: http
slug: ribbon-health-authentication
source_filename: ribbon-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ribbon-health-h1-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ribbon-health-h1-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/authentication/ribbon-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- Provider Directory
- Insurance
- Clinical Data
- Care Navigation
- Eligibility
- Price Transparency
- Provider Search
- Health Plans
- Digital Health
---
