---
api_key_in:
- header
api_specs:
- filename: pay-i-anthropic-requests-api-openapi.yml
  format: yaml
  label: Pay-i Anthropic Requests API
  slug: pay-i-anthropic-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-anthropic-requests-api-openapi.yml
- filename: pay-i-aws-bedrock-requests-api-openapi.yml
  format: yaml
  label: Pay-i AWS Bedrock Requests API
  slug: pay-i-aws-bedrock-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-aws-bedrock-requests-api-openapi.yml
- filename: pay-i-azure-anthropic-requests-api-openapi.yml
  format: yaml
  label: Pay-i Azure Anthropic Requests API
  slug: pay-i-azure-anthropic-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-azure-anthropic-requests-api-openapi.yml
- filename: pay-i-azure-openai-requests-api-openapi.yml
  format: yaml
  label: Pay-i Azure OpenAI Requests API
  slug: pay-i-azure-openai-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-azure-openai-requests-api-openapi.yml
- filename: pay-i-categories-api-openapi.yml
  format: yaml
  label: Pay-i Categories API
  slug: pay-i-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-categories-api-openapi.yml
- filename: pay-i-google-vertex-requests-api-openapi.yml
  format: yaml
  label: Pay-i Google Vertex Requests API
  slug: pay-i-google-vertex-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-google-vertex-requests-api-openapi.yml
- filename: pay-i-ingest-events-api-openapi.yml
  format: yaml
  label: Pay-i Ingest Events API
  slug: pay-i-ingest-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-ingest-events-api-openapi.yml
- filename: pay-i-kpis-api-openapi.yml
  format: yaml
  label: Pay-i KP Is API
  slug: pay-i-kpis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-kpis-api-openapi.yml
- filename: pay-i-limits-api-openapi.yml
  format: yaml
  label: Pay-i Limits API
  slug: pay-i-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-limits-api-openapi.yml
- filename: pay-i-openai-requests-api-openapi.yml
  format: yaml
  label: Pay-i OpenAI Requests API
  slug: pay-i-openai-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-openai-requests-api-openapi.yml
- filename: pay-i-reports-api-openapi.yml
  format: yaml
  label: Pay-i Reports API
  slug: pay-i-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-reports-api-openapi.yml
- filename: pay-i-requests-api-openapi.yml
  format: yaml
  label: Pay-i Requests API
  slug: pay-i-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-requests-api-openapi.yml
- filename: pay-i-resources-api-openapi.yml
  format: yaml
  label: Pay-i Resources API
  slug: pay-i-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-resources-api-openapi.yml
- filename: pay-i-use-cases-api-openapi.yml
  format: yaml
  label: Pay-i Use Cases API
  slug: pay-i-use-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-use-cases-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pay I Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pay-i secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pay-i
provider_slug: pay-i
scheme_count: 1
schemes:
- description: 'Pay-I API Key. Example: "{apikey}"'
  in: header
  name: Pay_I_API_Key
  parameter: xProxy-api-key
  sources:
  - openapi/pay-i-openapi-original.json
  - openapi/pay-i-openapi.yml
  type: apiKey
slug: pay-i-authentication
source_filename: pay-i-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/pay-i-openapi-original.json, openapi/pay-i-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Pay_I_API_Key\n  type: apiKey\n  in: header\n  parameter: xProxy-api-key\n  description: 'Pay-I API Key. Example: \"{apikey}\"'\n  sources:\n  - openapi/pay-i-openapi-original.json\n  - openapi/pay-i-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/authentication/pay-i-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- FinOps
- Observability
- Cost Management
- Generative AI
- LLM
- Analytics
- Governance
- Metering
---
