---
anonymous_access: false
api_key_in: []
api_specs:
- filename: maddegen-art-pump-cortex-api-openapi.yml
  format: yaml
  label: maddegen-art Pump Cortex API
  slug: maddegen-art-pump-cortex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-pump-cortex-api-openapi.yml
- filename: maddegen-art-chain-cortex-api-openapi.yml
  format: yaml
  label: maddegen-art Chain Cortex API
  slug: maddegen-art-chain-cortex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-chain-cortex-api-openapi.yml
- filename: maddegen-art-forensics-lobe-api-openapi.yml
  format: yaml
  label: maddegen-art Forensics Lobe API
  slug: maddegen-art-forensics-lobe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-forensics-lobe-api-openapi.yml
- filename: maddegen-art-hub-api-openapi.yml
  format: yaml
  label: maddegen-art Hub API
  slug: maddegen-art-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-hub-api-openapi.yml
- filename: maddegen-art-knowledge-cortex-api-openapi.yml
  format: yaml
  label: maddegen-art Knowledge Cortex API
  slug: maddegen-art-knowledge-cortex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-knowledge-cortex-api-openapi.yml
- filename: maddegen-art-liquidity-lobe-api-openapi.yml
  format: yaml
  label: maddegen-art Liquidity Lobe API
  slug: maddegen-art-liquidity-lobe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-liquidity-lobe-api-openapi.yml
- filename: maddegen-art-market-stem-api-openapi.yml
  format: yaml
  label: maddegen-art Market Stem API
  slug: maddegen-art-market-stem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-market-stem-api-openapi.yml
- filename: maddegen-art-risk-amygdala-api-openapi.yml
  format: yaml
  label: maddegen-art Risk Amygdala API
  slug: maddegen-art-risk-amygdala-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-risk-amygdala-api-openapi.yml
- filename: maddegen-art-utility-cerebellum-api-openapi.yml
  format: yaml
  label: maddegen-art Utility Cerebellum API
  slug: maddegen-art-utility-cerebellum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-utility-cerebellum-api-openapi.yml
- filename: maddegen-art-web-senses-api-openapi.yml
  format: yaml
  label: maddegen-art Web Senses API
  slug: maddegen-art-web-senses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-web-senses-api-openapi.yml
- filename: maddegen-art-world-map-api-openapi.yml
  format: yaml
  label: maddegen-art World Map API
  slug: maddegen-art-world-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-world-map-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Maddegen Art Authentication
name_suffix: Authentication
oauth_flows: []
overview: maddegen-art declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: maddegen-art
provider_slug: maddegen-art
scheme_count: 1
schemes:
- description: Bearer hk_… prepaid credit key (POST /hub/api/v1/keys). Paid tools also accept it instead of x402.
  in: header
  name: Authorization
  type: apiKey
slug: maddegen-art-authentication
source_filename: maddegen-art-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: https://augur-trade.com/hub/openapi.json\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer hk_… prepaid credit key (POST /hub/api/v1/keys). Paid tools also accept it instead of x402.\n"
source_yaml_url: https://artifacts.apis.io/maddegen-art/authentication/maddegen-art-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
