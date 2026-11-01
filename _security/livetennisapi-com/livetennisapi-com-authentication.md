---
anonymous_access: false
api_key_in: []
api_specs:
- filename: livetennisapi-com-broadcast-api-openapi.yml
  format: yaml
  label: Live Tennis API Broadcast API
  slug: livetennisapi-com-broadcast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-broadcast-api-openapi.yml
- filename: livetennisapi-com-charting-api-openapi.yml
  format: yaml
  label: Live Tennis API Charting API
  slug: livetennisapi-com-charting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-charting-api-openapi.yml
- filename: livetennisapi-com-events-api-openapi.yml
  format: yaml
  label: Live Tennis API Events API
  slug: livetennisapi-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-events-api-openapi.yml
- filename: livetennisapi-com-fixtures-api-openapi.yml
  format: yaml
  label: Live Tennis API Fixtures API
  slug: livetennisapi-com-fixtures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-fixtures-api-openapi.yml
- filename: livetennisapi-com-h2h-api-openapi.yml
  format: yaml
  label: Live Tennis API H2h API
  slug: livetennisapi-com-h2h-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-h2h-api-openapi.yml
- filename: livetennisapi-com-health-api-openapi.yml
  format: yaml
  label: Live Tennis API Health API
  slug: livetennisapi-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-health-api-openapi.yml
- filename: livetennisapi-com-history-api-openapi.yml
  format: yaml
  label: Live Tennis API History API
  slug: livetennisapi-com-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-history-api-openapi.yml
- filename: livetennisapi-com-markets-api-openapi.yml
  format: yaml
  label: Live Tennis API Markets API
  slug: livetennisapi-com-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-markets-api-openapi.yml
- filename: livetennisapi-com-matches-api-openapi.yml
  format: yaml
  label: Live Tennis API Matches API
  slug: livetennisapi-com-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-matches-api-openapi.yml
- filename: livetennisapi-com-players-api-openapi.yml
  format: yaml
  label: Live Tennis API Players API
  slug: livetennisapi-com-players-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-players-api-openapi.yml
- filename: livetennisapi-com-rally-api-openapi.yml
  format: yaml
  label: Live Tennis API Rally API
  slug: livetennisapi-com-rally-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-rally-api-openapi.yml
- filename: livetennisapi-com-rankings-api-openapi.yml
  format: yaml
  label: Live Tennis API Rankings API
  slug: livetennisapi-com-rankings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-rankings-api-openapi.yml
- filename: livetennisapi-com-tournaments-api-openapi.yml
  format: yaml
  label: Live Tennis API Tournaments API
  slug: livetennisapi-com-tournaments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-tournaments-api-openapi.yml
- filename: livetennisapi-com-usage-api-openapi.yml
  format: yaml
  label: Live Tennis API Usage API
  slug: livetennisapi-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-usage-api-openapi.yml
- filename: livetennisapi-com-webhooks-api-openapi.yml
  format: yaml
  label: Live Tennis API Webhooks API
  slug: livetennisapi-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-webhooks-api-openapi.yml
- filename: livetennisapi-com-ws-token-api-openapi.yml
  format: yaml
  label: Live Tennis API Ws Token API
  slug: livetennisapi-com-ws-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/livetennisapi-com/openapi/livetennisapi-com-ws-token-api-openapi.yml
auth_types: []
description: Live Tennis API uses a simple API key authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Livetennisapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Live Tennis API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Live Tennis API
provider_slug: livetennisapi-com
scheme_count: 1
schemes:
- evidence: Send your key as X-API-Key on every request.
  header: X-API-Key
  how_to_obtain: Free key can be obtained via the "Get a free key" link in the documentation.
  location: header
  name: X-API-Key
  type: apiKey
slug: livetennisapi-com-authentication
source_filename: livetennisapi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.livetennisapi.com/auth-quota-and-health.html
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.livetennisapi.com/auth-quota-and-health.html\nsources:\n- https://docs.livetennisapi.com/auth-quota-and-health.html\ndescription: Live Tennis API uses a simple API key authentication.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Send your key as X-API-Key on every request.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Free key can be obtained via the \"Get a free key\" link in the documentation.\nnote: No OAuth2, HTTP Bearer, or other authentication schemes are documented on the page.\ndocs: https://docs.livetennisapi.com/auth-quota-and-health.html\n"
source_yaml_url: https://artifacts.apis.io/livetennisapi-com/authentication/livetennisapi-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Sports
- Data
- Real-time
- API
- Tennis
---
