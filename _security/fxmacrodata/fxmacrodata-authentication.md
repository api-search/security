---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fxmacrodata-announcements-api-openapi.yml
  format: yaml
  label: FXMacroData Announcements API
  slug: fxmacrodata-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-announcements-api-openapi.yml
- filename: fxmacrodata-calendar-api-openapi.yml
  format: yaml
  label: FXMacroData Calendar API
  slug: fxmacrodata-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-calendar-api-openapi.yml
- filename: fxmacrodata-commodities-api-openapi.yml
  format: yaml
  label: FXMacroData Commodities API
  slug: fxmacrodata-commodities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-commodities-api-openapi.yml
- filename: fxmacrodata-data-catalogue-api-openapi.yml
  format: yaml
  label: FXMacroData Data Catalogue API
  slug: fxmacrodata-data-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-data-catalogue-api-openapi.yml
- filename: fxmacrodata-factors-api-openapi.yml
  format: yaml
  label: FXMacroData Factors API
  slug: fxmacrodata-factors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-factors-api-openapi.yml
- filename: fxmacrodata-fx-markets-api-openapi.yml
  format: yaml
  label: FXMacroData Fx Markets API
  slug: fxmacrodata-fx-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-fx-markets-api-openapi.yml
- filename: fxmacrodata-health-api-openapi.yml
  format: yaml
  label: FXMacroData Health API
  slug: fxmacrodata-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-health-api-openapi.yml
- filename: fxmacrodata-monetary-policy-api-openapi.yml
  format: yaml
  label: FXMacroData Monetary Policy API
  slug: fxmacrodata-monetary-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-monetary-policy-api-openapi.yml
- filename: fxmacrodata-predictions-api-openapi.yml
  format: yaml
  label: FXMacroData Predictions API
  slug: fxmacrodata-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-predictions-api-openapi.yml
- filename: fxmacrodata-press-releases-api-openapi.yml
  format: yaml
  label: FXMacroData Press Releases API
  slug: fxmacrodata-press-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-press-releases-api-openapi.yml
- filename: fxmacrodata-settlement-api-openapi.yml
  format: yaml
  label: FXMacroData Settlement API
  slug: fxmacrodata-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-settlement-api-openapi.yml
auth_types: []
description: FXMacroData uses API key authentication via a custom header and also accepts the same key as a Bearer token.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fxmacrodata Authentication
name_suffix: Authentication
oauth_flows: []
overview: FXMacroData declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FXMacroData
provider_slug: fxmacrodata
scheme_count: 2
schemes:
- evidence: "Authentication\n X-API-Key: YOUR_API_KEY"
  header: X-API-Key
  how_to_obtain: Obtain an API key from your FXMacroData account or subscription.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Use the same API key as a Bearer token.
  location: header
  name: Authorization
  type: http-bearer
slug: fxmacrodata-authentication
source_filename: fxmacrodata-authentication.yml
source_heading: Authentication Profile
source_url: https://fxmacrodata.com/documentation/quickstart
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fxmacrodata.com/documentation/quickstart\nsources:\n- https://fxmacrodata.com/documentation/quickstart\n- https://fxmacrodata.com/documentation/mcp-server\n- https://fxmacrodata.com/es/documentation/quickstart\n- https://fxmacrodata.com/pt/documentation/quickstart\ndescription: FXMacroData uses API key authentication via a custom header and also accepts the same key as a Bearer token.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: \"Authentication\\n X-API-Key: YOUR_API_KEY\"\n  location: header\n  header: X-API-Key\n  how_to_obtain: Obtain an API key from your FXMacroData account or subscription.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Use the same API key as a Bearer token.\nnote: No OAuth2 flows, client credentials, or other authentication mechanisms\
  \ are documented on the referenced pages.\ndocs: https://fxmacrodata.com/documentation/quickstart\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/authentication/fxmacrodata-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Data
- API
- FX
---
