---
api_key_in:
- header
api_specs:
- filename: glassnode-addresses-api-openapi.yml
  format: yaml
  label: Glassnode Addresses API
  slug: glassnode-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-addresses-api-openapi.yml
- filename: glassnode-derivatives-api-openapi.yml
  format: yaml
  label: Glassnode Derivatives API
  slug: glassnode-derivatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-derivatives-api-openapi.yml
- filename: glassnode-distribution-api-openapi.yml
  format: yaml
  label: Glassnode Distribution API
  slug: glassnode-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-distribution-api-openapi.yml
- filename: glassnode-indicators-api-openapi.yml
  format: yaml
  label: Glassnode Indicators API
  slug: glassnode-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-indicators-api-openapi.yml
- filename: glassnode-macro-api-openapi.yml
  format: yaml
  label: Glassnode Macro API
  slug: glassnode-macro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-macro-api-openapi.yml
- filename: glassnode-market-api-openapi.yml
  format: yaml
  label: Glassnode Market API
  slug: glassnode-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-market-api-openapi.yml
- filename: glassnode-metadata-api-openapi.yml
  format: yaml
  label: Glassnode Metadata API
  slug: glassnode-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-metadata-api-openapi.yml
- filename: glassnode-options-api-openapi.yml
  format: yaml
  label: Glassnode Options API
  slug: glassnode-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-options-api-openapi.yml
- filename: glassnode-supply-api-openapi.yml
  format: yaml
  label: Glassnode Supply API
  slug: glassnode-supply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-supply-api-openapi.yml
- filename: glassnode-transactions-api-openapi.yml
  format: yaml
  label: Glassnode Transactions API
  slug: glassnode-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-transactions-api-openapi.yml
- filename: glassnode-treasuries-api-openapi.yml
  format: yaml
  label: Glassnode Treasuries API
  slug: glassnode-treasuries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-treasuries-api-openapi.yml
- filename: glassnode-user-api-openapi.yml
  format: yaml
  label: Glassnode User API
  slug: glassnode-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Glassnode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glassnode secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Glassnode
provider_slug: glassnode
scheme_count: 1
schemes:
- description: Glassnode API key with institutional or paid plan.
  in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/glassnode-openapi.yml
  type: apiKey
slug: glassnode-authentication
source_filename: glassnode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/glassnode-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Glassnode API key with institutional or paid plan.\n  sources:\n  - openapi/glassnode-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/authentication/glassnode-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Crypto
- On-Chain
- Analytics
- Metrics
- Bitcoin
- Ethereum
- Institutional
---
