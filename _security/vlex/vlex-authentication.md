---
api_key_in:
- header
api_specs:
- filename: vlex-anonymization-api-openapi.yml
  format: yaml
  label: vLex Anonymization API
  slug: vlex-anonymization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vlex/refs/heads/main/openapi/vlex-anonymization-api-openapi.yml
- filename: vlex-citations-api-openapi.yml
  format: yaml
  label: vLex Citations API
  slug: vlex-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vlex/refs/heads/main/openapi/vlex-citations-api-openapi.yml
- filename: vlex-classification-api-openapi.yml
  format: yaml
  label: vLex Classification API
  slug: vlex-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vlex/refs/heads/main/openapi/vlex-classification-api-openapi.yml
- filename: vlex-documents-api-openapi.yml
  format: yaml
  label: vLex Documents API
  slug: vlex-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vlex/refs/heads/main/openapi/vlex-documents-api-openapi.yml
- filename: vlex-search-api-openapi.yml
  format: yaml
  label: vLex Search API
  slug: vlex-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vlex/refs/heads/main/openapi/vlex-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vlex Authentication
name_suffix: Authentication
oauth_flows: []
overview: vLex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: vLex
provider_slug: vlex
scheme_count: 1
schemes:
- description: vLex API subscription key obtained from the developer portal.
  in: header
  name: SubscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/vlex-iceberg-anonymization-openapi.yml
  - openapi/vlex-iceberg-legal-research-openapi.yml
  type: apiKey
slug: vlex-authentication
source_filename: vlex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vlex-iceberg-anonymization-openapi.yml, openapi/vlex-iceberg-legal-research-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SubscriptionKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: vLex API subscription key obtained from the developer portal.\n  sources:\n  - openapi/vlex-iceberg-anonymization-openapi.yml\n  - openapi/vlex-iceberg-legal-research-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vlex/refs/heads/main/authentication/vlex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Classification
- Legal Research
- Legal Tech
- Natural Language Processing
- Privacy
---
