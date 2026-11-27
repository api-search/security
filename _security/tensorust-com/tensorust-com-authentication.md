---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: tensorust-com-crates-api-openapi.yml
  format: yaml
  label: Tensorust LLC Crates API
  slug: tensorust-com-crates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-crates-api-openapi.yml
- filename: tensorust-com-data-api-openapi.yml
  format: yaml
  label: Tensorust LLC Data API
  slug: tensorust-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-data-api-openapi.yml
- filename: tensorust-com-datasets-api-openapi.yml
  format: yaml
  label: Tensorust LLC Datasets API
  slug: tensorust-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-datasets-api-openapi.yml
- filename: tensorust-com-healthcare-api-openapi.yml
  format: yaml
  label: Tensorust LLC Healthcare API
  slug: tensorust-com-healthcare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-healthcare-api-openapi.yml
- filename: tensorust-com-history-api-openapi.yml
  format: yaml
  label: Tensorust LLC History API
  slug: tensorust-com-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-history-api-openapi.yml
- filename: tensorust-com-llm-api-openapi.yml
  format: yaml
  label: Tensorust LLC Llm API
  slug: tensorust-com-llm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-llm-api-openapi.yml
- filename: tensorust-com-manual-api-openapi.yml
  format: yaml
  label: Tensorust LLC Manual API
  slug: tensorust-com-manual-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-manual-api-openapi.yml
- filename: tensorust-com-ontology-api-openapi.yml
  format: yaml
  label: Tensorust LLC Ontology API
  slug: tensorust-com-ontology-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-ontology-api-openapi.yml
- filename: tensorust-com-openapi-json-api-openapi.yml
  format: yaml
  label: Tensorust LLC Openapi.json API
  slug: tensorust-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-openapi-json-api-openapi.yml
- filename: tensorust-com-private-credit-api-openapi.yml
  format: yaml
  label: Tensorust LLC Private Credit API
  slug: tensorust-com-private-credit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-private-credit-api-openapi.yml
- filename: tensorust-com-property-api-openapi.yml
  format: yaml
  label: Tensorust LLC Property API
  slug: tensorust-com-property-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-property-api-openapi.yml
- filename: tensorust-com-records-api-openapi.yml
  format: yaml
  label: Tensorust LLC Records API
  slug: tensorust-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-records-api-openapi.yml
- filename: tensorust-com-reports-api-openapi.yml
  format: yaml
  label: Tensorust LLC Reports API
  slug: tensorust-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-reports-api-openapi.yml
- filename: tensorust-com-research-api-openapi.yml
  format: yaml
  label: Tensorust LLC Research API
  slug: tensorust-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-research-api-openapi.yml
- filename: tensorust-com-research-exposure-api-openapi.yml
  format: yaml
  label: Tensorust LLC Research Exposure API
  slug: tensorust-com-research-exposure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-research-exposure-api-openapi.yml
- filename: tensorust-com-restricted-vendors-api-openapi.yml
  format: yaml
  label: Tensorust LLC Restricted Vendors API
  slug: tensorust-com-restricted-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-restricted-vendors-api-openapi.yml
- filename: tensorust-com-search-api-openapi.yml
  format: yaml
  label: Tensorust LLC Search API
  slug: tensorust-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-search-api-openapi.yml
- filename: tensorust-com-tools-api-openapi.yml
  format: yaml
  label: Tensorust LLC Tools API
  slug: tensorust-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tensorust-com/openapi/tensorust-com-tools-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Tensorust LLC Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tensorust LLC secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tensorust LLC
provider_slug: tensorust-com
scheme_count: 2
schemes:
- description: Enterprise API key tdk_... (https://tensorust.com/offers/enterprise-api/)
  name: bearer
  scheme: bearer
  sources:
  - openapi/api_tensorust_com.json
  - openapi/shop_tensorust_com.json
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/api_tensorust_com.json
  - openapi/shop_tensorust_com.json
  type: apiKey
slug: tensorust-com-authentication
source_filename: tensorust-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/api_tensorust_com.json, openapi/shop_tensorust_com.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Enterprise API key tdk_... (https://tensorust.com/offers/enterprise-api/)\n  sources:\n  - openapi/api_tensorust_com.json\n  - openapi/shop_tensorust_com.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/api_tensorust_com.json\n  - openapi/shop_tensorust_com.json\n"
source_yaml_url: https://artifacts.apis.io/tensorust-com/authentication/tensorust-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data
- Datasets
- Money Recovery
- Compliance
- AI Pricing
- Rust Crates
---
