---
anonymous_access: false
api_key_in: []
api_specs:
- filename: prospectapis-health-api-openapi.yml
  format: yaml
  label: ProspectAPIs Health API
  slug: prospectapis-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/openapi/prospectapis-health-api-openapi.yml
- filename: prospectapis-pricing-api-openapi.yml
  format: yaml
  label: ProspectAPIs Pricing API
  slug: prospectapis-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/openapi/prospectapis-pricing-api-openapi.yml
- filename: prospectapis-prospectapis-api-api-openapi.yml
  format: yaml
  label: ProspectAPIs ProspectAPIs API
  slug: prospectapis-prospectapis-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/openapi/prospectapis-prospectapis-api-api-openapi.yml
- filename: prospectapis-watchlists-api-openapi.yml
  format: yaml
  label: ProspectAPIs Watchlists API
  slug: prospectapis-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/openapi/prospectapis-watchlists-api-openapi.yml
auth_types: []
description: Authentication Send the key in the Authorization header as a Bearer token on every /v1 request except GET /v1/version .
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Prospectapis Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProspectAPIs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ProspectAPIs
provider_slug: prospectapis
scheme_count: 1
schemes:
- evidence: Authentication Send the key in the Authorization header as a Bearer token on every /v1 request except GET /v1/version .
  header: Authorization
  how_to_obtain: Create an account, open API keys and create one.
  location: header
  name: Bearer
  type: http-bearer
slug: prospectapis-authentication
source_filename: prospectapis-authentication.yml
source_heading: Authentication Profile
source_url: https://prospectapis.com/docs
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://prospectapis.com/docs\nsources:\n- https://prospectapis.com/docs\ndescription: Authentication Send the key in the Authorization header as a Bearer token on every /v1 request except GET /v1/version .\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Authentication Send the key in the Authorization header as a Bearer token on every /v1 request except GET /v1/version .\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account, open API keys and create one.\ndocs: https://prospectapis.com/docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/authentication/prospectapis-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Funding
- Research
- Data
---
