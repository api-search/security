---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sochain-com-account-api-openapi.yml
  format: yaml
  label: sochain-com Account API
  slug: sochain-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sochain-com/openapi/sochain-com-account-api-openapi.yml
- filename: sochain-com-addresses-api-openapi.yml
  format: yaml
  label: sochain-com Addresses API
  slug: sochain-com-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sochain-com/openapi/sochain-com-addresses-api-openapi.yml
- filename: sochain-com-blocks-api-openapi.yml
  format: yaml
  label: sochain-com Blocks API
  slug: sochain-com-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sochain-com/openapi/sochain-com-blocks-api-openapi.yml
- filename: sochain-com-buckets-api-openapi.yml
  format: yaml
  label: sochain-com Buckets API
  slug: sochain-com-buckets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sochain-com/openapi/sochain-com-buckets-api-openapi.yml
- filename: sochain-com-charts-api-openapi.yml
  format: yaml
  label: sochain-com Charts API
  slug: sochain-com-charts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sochain-com/openapi/sochain-com-charts-api-openapi.yml
- filename: sochain-com-network-price-api-openapi.yml
  format: yaml
  label: sochain-com Network & price API
  slug: sochain-com-network-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sochain-com/openapi/sochain-com-network-price-api-openapi.yml
- filename: sochain-com-sochain-api-api-openapi.yml
  format: yaml
  label: sochain-com SoChain API
  slug: sochain-com-sochain-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sochain-com/openapi/sochain-com-sochain-api-api-openapi.yml
- filename: sochain-com-transactions-api-openapi.yml
  format: yaml
  label: sochain-com Transactions API
  slug: sochain-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sochain-com/openapi/sochain-com-transactions-api-openapi.yml
- filename: sochain-com-webhooks-api-openapi.yml
  format: yaml
  label: sochain-com Webhooks API
  slug: sochain-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sochain-com/openapi/sochain-com-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Sochain Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: sochain-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: sochain-com
provider_slug: sochain-com
scheme_count: 2
schemes:
- description: Your key, from the dashboard.
  in: header
  name: API-KEY
  type: apiKey
- description: Your key as a URL parameter, for lookups (GET) from tools that can't send a header.
  in: query
  name: api_key
  type: apiKey
slug: sochain-com-authentication
source_filename: sochain-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://sochain.com/docs/authentication\nschemes:\n  - type: apiKey\n    name: API-KEY\n    in: header\n    description: Your key, from the dashboard.\n  - type: apiKey\n    name: api_key\n    in: query\n    description: Your key as a URL parameter, for lookups (GET) from tools that can't send a header.\n"
source_yaml_url: https://artifacts.apis.io/sochain-com/authentication/sochain-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Blockchain
- Explorer
- API
- Cryptocurrency
- Finance
---
