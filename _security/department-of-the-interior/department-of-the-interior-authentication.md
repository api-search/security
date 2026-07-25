---
api_key_in:
- query
api_specs:
- filename: department-of-the-interior-alerts-api-openapi.yml
  format: yaml
  label: Department of the Interior Alerts API
  slug: department-of-the-interior-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-alerts-api-openapi.yml
- filename: department-of-the-interior-articles-api-openapi.yml
  format: yaml
  label: Department of the Interior Articles API
  slug: department-of-the-interior-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-articles-api-openapi.yml
- filename: department-of-the-interior-campgrounds-api-openapi.yml
  format: yaml
  label: Department of the Interior Campgrounds API
  slug: department-of-the-interior-campgrounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-campgrounds-api-openapi.yml
- filename: department-of-the-interior-counts-api-openapi.yml
  format: yaml
  label: Department of the Interior Counts API
  slug: department-of-the-interior-counts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-counts-api-openapi.yml
- filename: department-of-the-interior-dailyvalues-api-openapi.yml
  format: yaml
  label: Department of the Interior DailyValues API
  slug: department-of-the-interior-dailyvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-dailyvalues-api-openapi.yml
- filename: department-of-the-interior-events-api-openapi.yml
  format: yaml
  label: Department of the Interior Events API
  slug: department-of-the-interior-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-events-api-openapi.yml
- filename: department-of-the-interior-instantaneousvalues-api-openapi.yml
  format: yaml
  label: Department of the Interior InstantaneousValues API
  slug: department-of-the-interior-instantaneousvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-instantaneousvalues-api-openapi.yml
- filename: department-of-the-interior-parks-api-openapi.yml
  format: yaml
  label: Department of the Interior Parks API
  slug: department-of-the-interior-parks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-parks-api-openapi.yml
- filename: department-of-the-interior-sites-api-openapi.yml
  format: yaml
  label: Department of the Interior Sites API
  slug: department-of-the-interior-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-sites-api-openapi.yml
- filename: department-of-the-interior-visitorcenters-api-openapi.yml
  format: yaml
  label: Department of the Interior VisitorCenters API
  slug: department-of-the-interior-visitorcenters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-visitorcenters-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Department Of The Interior Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of the Interior secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Department of the Interior
provider_slug: department-of-the-interior
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/nps-data-api-openapi.yml
  type: apiKey
slug: department-of-the-interior-authentication
source_filename: department-of-the-interior-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nps-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/nps-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/authentication/department-of-the-interior-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Public Lands
- Natural Resources
- Geospatial
---
