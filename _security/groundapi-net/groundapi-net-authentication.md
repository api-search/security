---
anonymous_access: false
api_key_in: []
api_specs:
- filename: groundapi-net-finance-data-api-openapi.yml
  format: yaml
  label: GroundAPI Finance - Data API
  slug: groundapi-net-finance-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundapi-net/openapi/groundapi-net-finance-data-api-openapi.yml
- filename: groundapi-net-finance-market-api-openapi.yml
  format: yaml
  label: GroundAPI Finance - Market API
  slug: groundapi-net-finance-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundapi-net/openapi/groundapi-net-finance-market-api-openapi.yml
- filename: groundapi-net-finance-search-api-openapi.yml
  format: yaml
  label: GroundAPI Finance - Search API
  slug: groundapi-net-finance-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundapi-net/openapi/groundapi-net-finance-search-api-openapi.yml
- filename: groundapi-net-finance-stock-api-openapi.yml
  format: yaml
  label: GroundAPI Finance - Stock API
  slug: groundapi-net-finance-stock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundapi-net/openapi/groundapi-net-finance-stock-api-openapi.yml
auth_types: []
description: Authentication methods for GroundAPI
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GroundAPI Authentication
name_suffix: Authentication
oauth_flows: []
overview: GroundAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GroundAPI
provider_slug: groundapi-net
scheme_count: 1
schemes:
- evidence: All data endpoints are authenticated via the X-API-Key HTTP header.
  header: X-API-Key
  how_to_obtain: Log in to the GroundAPI Dashboard, click "Create New Key", enter a key name, and copy the shown key.
  location: header
  name: API Key
  type: apiKey
slug: groundapi-net-authentication
source_filename: groundapi-net-authentication.yml
source_heading: Authentication Profile
source_url: https://groundapi.net/en/documentation/authentication
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://groundapi.net/en/documentation/authentication\nsources:\n- https://groundapi.net/en/documentation/authentication\n- https://groundapi.net/en/documentation/authentication\n- https://groundapi.net/en/documentation/quick-start\n- https://groundapi.net/en/blog/rest-api-quick-start\ndescription: Authentication methods for GroundAPI\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All data endpoints are authenticated via the X-API-Key HTTP header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Log in to the GroundAPI Dashboard, click \"Create New Key\", enter a key name, and copy the shown key.\nnote: No OAuth2 or other authentication schemes are documented on the provided pages.\ndocs: https://groundapi.net/en/documentation/authentication\n"
source_yaml_url: https://artifacts.apis.io/groundapi-net/authentication/groundapi-net-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Artificial Intelligence
- Data
- Market Data
- China
---
