---
api_key_in: []
api_specs:
- filename: ibm-api-keys-api-openapi.yml
  format: yaml
  label: IBM API Keys API
  slug: ibm-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-api-keys-api-openapi.yml
- filename: ibm-claim-rules-api-openapi.yml
  format: yaml
  label: IBM Claim Rules API
  slug: ibm-claim-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-claim-rules-api-openapi.yml
- filename: ibm-policies-api-openapi.yml
  format: yaml
  label: IBM Policies API
  slug: ibm-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-policies-api-openapi.yml
- filename: ibm-roles-api-openapi.yml
  format: yaml
  label: IBM Roles API
  slug: ibm-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-roles-api-openapi.yml
- filename: ibm-service-ids-api-openapi.yml
  format: yaml
  label: IBM Service IDs API
  slug: ibm-service-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-service-ids-api-openapi.yml
- filename: ibm-tokens-api-openapi.yml
  format: yaml
  label: IBM Tokens API
  slug: ibm-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-tokens-api-openapi.yml
- filename: ibm-trusted-profiles-api-openapi.yml
  format: yaml
  label: IBM Trusted Profiles API
  slug: ibm-trusted-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-trusted-profiles-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ibm Authentication
name_suffix: Authentication
oauth_flows: []
overview: IBM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IBM
provider_slug: ibm
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'IAM access token obtained from the /identity/token endpoint. Pass as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ibm-cloud-iam.yml
  type: http
slug: ibm-authentication
source_filename: ibm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ibm-cloud-iam.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'IAM access token obtained from the /identity/token endpoint. Pass as Authorization:\n    Bearer <token>.'\n  sources:\n  - openapi/ibm-cloud-iam.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/authentication/ibm-authentication.yml
summary_line: http · 1 scheme
tags:
- API Management
- Artificial Intelligence
- Billing
- Cloud Computing
- Containers
- Data Governance
- Databases
- DevOps
- Enterprise
- Generative AI
- Hybrid Cloud
- Infrastructure
- Machine Learning
- Networking
- Observability
- Security
- Serverless
- Storage
- Watson
- Watsonx
- Fortune 100
---
