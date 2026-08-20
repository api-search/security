---
api_key_in:
- header
api_specs:
- filename: amazon-supply-chain-bill-of-materials-api-openapi.yml
  format: yaml
  label: Amazon Supply Chain Bill of Materials API
  slug: amazon-supply-chain-bill-of-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/openapi/amazon-supply-chain-bill-of-materials-api-openapi.yml
- filename: amazon-supply-chain-data-integration-events-api-openapi.yml
  format: yaml
  label: Amazon Supply Chain Data Integration Events API
  slug: amazon-supply-chain-data-integration-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/openapi/amazon-supply-chain-data-integration-events-api-openapi.yml
- filename: amazon-supply-chain-data-integration-flows-api-openapi.yml
  format: yaml
  label: Amazon Supply Chain Data Integration Flows API
  slug: amazon-supply-chain-data-integration-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/openapi/amazon-supply-chain-data-integration-flows-api-openapi.yml
- filename: amazon-supply-chain-data-lake-api-openapi.yml
  format: yaml
  label: Amazon Supply Chain Data Lake API
  slug: amazon-supply-chain-data-lake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/openapi/amazon-supply-chain-data-lake-api-openapi.yml
- filename: amazon-supply-chain-instances-api-openapi.yml
  format: yaml
  label: Amazon Supply Chain Instances API
  slug: amazon-supply-chain-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/openapi/amazon-supply-chain-instances-api-openapi.yml
- filename: amazon-supply-chain-tags-api-openapi.yml
  format: yaml
  label: Amazon Supply Chain Tags API
  slug: amazon-supply-chain-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/openapi/amazon-supply-chain-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Supply Chain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Supply Chain secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Supply Chain
provider_slug: amazon-supply-chain
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-supply-chain.yaml
  type: apiKey
slug: amazon-supply-chain-authentication
source_filename: amazon-supply-chain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-supply-chain.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-supply-chain.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/authentication/amazon-supply-chain-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ERP Integration
- Logistics
- Machine-Learning
- Supply Chain
---
