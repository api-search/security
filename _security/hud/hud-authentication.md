---
api_key_in: []
api_specs:
- filename: hud-chas-api-openapi.yml
  format: yaml
  label: HUD - US Department of Housing and Urban Development CHAS API
  slug: hud-chas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-chas-api-openapi.yml
- filename: hud-fair-market-rents-api-openapi.yml
  format: yaml
  label: HUD - US Department of Housing and Urban Development Fair Market Rents API
  slug: hud-fair-market-rents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-fair-market-rents-api-openapi.yml
- filename: hud-housing-counseling-api-openapi.yml
  format: yaml
  label: HUD - US Department of Housing and Urban Development Housing Counseling API
  slug: hud-housing-counseling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-housing-counseling-api-openapi.yml
- filename: hud-income-limits-api-openapi.yml
  format: yaml
  label: HUD - US Department of Housing and Urban Development Income Limits API
  slug: hud-income-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-income-limits-api-openapi.yml
- filename: hud-zip-code-crosswalk-api-openapi.yml
  format: yaml
  label: HUD - US Department of Housing and Urban Development ZIP Code Crosswalk API
  slug: hud-zip-code-crosswalk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hud/refs/heads/main/openapi/hud-zip-code-crosswalk-api-openapi.yml
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
