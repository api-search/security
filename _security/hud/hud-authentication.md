---
api_key_in: []
api_specs:
- filename: hud-fair-market-rents-openapi.yml
  format: yaml
  label: HUD User Fair Market Rents API
  slug: hud-user-fair-market-rents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-fair-market-rents-openapi.yml
- filename: hud-income-limits-openapi.yml
  format: yaml
  label: HUD User Income Limits API
  slug: hud-user-income-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-income-limits-openapi.yml
- filename: hud-usps-zip-code-crosswalk-openapi.yml
  format: yaml
  label: HUD User USPS ZIP Code Crosswalk API
  slug: hud-user-usps-zip-code-crosswalk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-usps-zip-code-crosswalk-openapi.yml
- filename: hud-chas-openapi.yml
  format: yaml
  label: HUD User CHAS API
  slug: hud-user-chas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-chas-openapi.yml
- filename: hud-housing-counselor-search-openapi.yml
  format: yaml
  label: HUD Housing Counselor Search API
  slug: hud-housing-counselor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-housing-counselor-search-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hud Authentication
name_suffix: Authentication
oauth_flows: []
overview: HUD - US Department of Housing and Urban Development secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HUD - US Department of Housing and Urban Development
provider_slug: hud
scheme_count: 1
schemes:
- description: Bearer token obtained by registering at https://www.huduser.gov/hudapi/public/register
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hud-chas-openapi.yml
  - openapi/hud-fair-market-rents-openapi.yml
  - openapi/hud-income-limits-openapi.yml
  - openapi/hud-usps-zip-code-crosswalk-openapi.yml
  type: http
slug: hud-authentication
source_filename: hud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hud-chas-openapi.yml, openapi/hud-fair-market-rents-openapi.yml, openapi/hud-income-limits-openapi.yml,\n  openapi/hud-usps-zip-code-crosswalk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained by registering at https://www.huduser.gov/hudapi/public/register\n  sources:\n  - openapi/hud-chas-openapi.yml\n  - openapi/hud-fair-market-rents-openapi.yml\n  - openapi/hud-income-limits-openapi.yml\n  - openapi/hud-usps-zip-code-crosswalk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/authentication/hud-authentication.yml
summary_line: http · 1 scheme
tags:
- Housing
- Government
- Fair Market Rent
- Mortgage
- Community Development
- Public Housing
- Section 8
- Income Limits
---
