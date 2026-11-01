---
anonymous_access: false
api_key_in: []
api_specs:
- filename: regrow-ag-ogc-api-general-api-openapi.yml
  format: yaml
  label: Regrow OGC API - General API
  slug: regrow-ag-ogc-api-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-ogc-api-general-api-openapi.yml
- filename: regrow-ag-ogc-api-processes-api-openapi.yml
  format: yaml
  label: Regrow OGC API - Processes API
  slug: regrow-ag-ogc-api-processes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-ogc-api-processes-api-openapi.yml
- filename: regrow-ag-v0-explore-api-intervention-api-openapi.yml
  format: yaml
  label: Regrow V0 Explore API - Intervention API
  slug: regrow-ag-v0-explore-api-intervention-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v0-explore-api-intervention-api-openapi.yml
- filename: regrow-ag-v0-measure-api-intervention-api-openapi.yml
  format: yaml
  label: Regrow V0 Measure API - Intervention API
  slug: regrow-ag-v0-measure-api-intervention-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v0-measure-api-intervention-api-openapi.yml
- filename: regrow-ag-v0-measure-api-inventory-api-openapi.yml
  format: yaml
  label: Regrow V0 Measure API - Inventory API
  slug: regrow-ag-v0-measure-api-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v0-measure-api-inventory-api-openapi.yml
- filename: regrow-ag-v1-measure-api-enteric-api-openapi.yml
  format: yaml
  label: Regrow V1 Measure API - Enteric API
  slug: regrow-ag-v1-measure-api-enteric-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v1-measure-api-enteric-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Regrow Ag Authentication
name_suffix: Authentication
oauth_flows: []
overview: Regrow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Regrow
provider_slug: regrow-ag
scheme_count: 1
schemes:
- description: API key authentication for both Monitor API and Measure API
  docs: https://developers.regrow.ag/portals/api/sites/flurosat-154904-regrowdeveloper/liveportal/apis/monitor-v2/download_spec
  evidence:
  - Monitor API OpenAPI states "The Monitor API uses API keys to authenticate requests. To receive an API key, reach out to Regrow Support at support@regrow.ag. Include the API key as a `x-apikey` header for all API requests."
  - Measure API OpenAPI shows x-apikey header parameter required for all endpoints
  in: header
  name: x-apikey
  type: apiKey
slug: regrow-ag-authentication
source_filename: regrow-ag-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/regrow-ag-monitor-api-openapi.yml, openapi/regrow-ag-measure-api-openapi.yml\nschemes:\n  - type: apiKey\n    name: x-apikey\n    in: header\n    description: API key authentication for both Monitor API and Measure API\n    docs: https://developers.regrow.ag/portals/api/sites/flurosat-154904-regrowdeveloper/liveportal/apis/monitor-v2/download_spec\n    evidence:\n      - Monitor API OpenAPI states \"The Monitor API uses API keys to authenticate requests. To receive an API key, reach out to Regrow Support at support@regrow.ag. Include the API key as a `x-apikey` header for all API requests.\"\n      - Measure API OpenAPI shows x-apikey header parameter required for all endpoints\nnote: Both APIs use API key authentication via x-apikey header. No OAuth or other authentication schemes documented in public OpenAPI specifications."
source_yaml_url: https://artifacts.apis.io/regrow-ag/authentication/regrow-ag-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Agriculture
- Sustainability
- Greenhouse Gas Emissions
- Carbon
- Regenerative Agriculture
- Remote Sensing
- Climate
---
