---
anonymous_access: false
api_key_in: []
api_specs:
- filename: besot-com-artists-api-openapi.yml
  format: yaml
  label: besot Artists API
  slug: besot-com-artists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-artists-api-openapi.yml
- filename: besot-com-categories-api-openapi.yml
  format: yaml
  label: besot Categories API
  slug: besot-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-categories-api-openapi.yml
- filename: besot-com-collections-api-openapi.yml
  format: yaml
  label: besot Collections API
  slug: besot-com-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-collections-api-openapi.yml
- filename: besot-com-designers-api-openapi.yml
  format: yaml
  label: besot Designers API
  slug: besot-com-designers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-designers-api-openapi.yml
- filename: besot-com-facets-api-openapi.yml
  format: yaml
  label: besot Facets API
  slug: besot-com-facets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-facets-api-openapi.yml
- filename: besot-com-networks-api-openapi.yml
  format: yaml
  label: besot Networks API
  slug: besot-com-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-networks-api-openapi.yml
- filename: besot-com-pieces-api-openapi.yml
  format: yaml
  label: besot Pieces API
  slug: besot-com-pieces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-pieces-api-openapi.yml
- filename: besot-com-programs-api-openapi.yml
  format: yaml
  label: besot Programs API
  slug: besot-com-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-programs-api-openapi.yml
- filename: besot-com-search-api-openapi.yml
  format: yaml
  label: besot Search API
  slug: besot-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-search-api-openapi.yml
- filename: besot-com-stats-api-openapi.yml
  format: yaml
  label: besot Stats API
  slug: besot-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-stats-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Besot Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: besot declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: besot
provider_slug: besot-com
scheme_count: 2
schemes:
- description: Your API key as a Bearer token. Get a free key at /developers.
  id: ApiKeyBearer
  scheme: bearer
  type: http
- description: Your API key (alternative to the Authorization header).
  id: ApiKeyHeader
  in: header
  name: x-api-key
  type: apiKey
slug: besot-com-authentication
source_filename: besot-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: https://besot.com/catalogue/openapi.json\nschemes:\n  - id: ApiKeyBearer\n    type: http\n    scheme: bearer\n    description: \"Your API key as a Bearer token. Get a free key at /developers.\"\n  - id: ApiKeyHeader\n    type: apiKey\n    in: header\n    name: x-api-key\n    description: \"Your API key (alternative to the Authorization header).\"\n"
source_yaml_url: https://artifacts.apis.io/besot-com/authentication/besot-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Fashion
- Resale
- Catalog
- Fandom
- Clothing
---
