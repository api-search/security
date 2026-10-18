---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: phala-apps-api-openapi.yml
  format: yaml
  label: Phala Network Apps API
  slug: phala-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-api-openapi.yml
- filename: phala-apps-kms-info-api-openapi.yml
  format: yaml
  label: Phala Network Apps Kms Info API
  slug: phala-apps-kms-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-kms-info-api-openapi.yml
- filename: phala-apps-pending-updates-api-openapi.yml
  format: yaml
  label: Phala Network Apps Pending Updates API
  slug: phala-apps-pending-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-pending-updates-api-openapi.yml
- filename: phala-attestations-api-openapi.yml
  format: yaml
  label: Phala Network Attestations API
  slug: phala-attestations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-attestations-api-openapi.yml
- filename: phala-cvms-api-openapi.yml
  format: yaml
  label: Phala Network CVMs API
  slug: phala-cvms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-cvms-api-openapi.yml
- filename: phala-cvms-network-config-api-openapi.yml
  format: yaml
  label: Phala Network Cvms Network Config API
  slug: phala-cvms-network-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-cvms-network-config-api-openapi.yml
- filename: phala-instance-types-api-openapi.yml
  format: yaml
  label: Phala Network Instance Types API
  slug: phala-instance-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-instance-types-api-openapi.yml
- filename: phala-kms-api-openapi.yml
  format: yaml
  label: Phala Network KMS API
  slug: phala-kms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-kms-api-openapi.yml
- filename: phala-ssh-keys-api-openapi.yml
  format: yaml
  label: Phala Network SSH Keys API
  slug: phala-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-ssh-keys-api-openapi.yml
- filename: phala-webhooks-api-openapi.yml
  format: yaml
  label: Phala Network Webhooks API
  slug: phala-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-webhooks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Phala Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Phala Network secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Phala Network
provider_slug: phala
scheme_count: 2
schemes:
- flows:
  - flow: authorizationCode
    scopes: 0
    tokenUrl: token
  name: OAuth2AuthorizationCodeBearer
  sources:
  - openapi/phala-cloud-api-openapi.yml
  type: oauth2
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/phala-cloud-api-openapi.yml
  type: apiKey
slug: phala-authentication
source_filename: phala-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/phala-cloud-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2AuthorizationCodeBearer\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    tokenUrl: token\n    scopes: 0\n  sources:\n  - openapi/phala-cloud-api-openapi.yml\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/phala-cloud-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/authentication/phala-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Confidential Computing
- Trusted Execution Environments
- Inference
- Cloud Infrastructure
- Attestation
- LLM Router
---
