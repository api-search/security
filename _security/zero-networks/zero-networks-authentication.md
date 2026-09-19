---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: zero-networks-ae-exclusions-api-openapi.yml
  format: yaml
  label: Zero Networks AE Exclusions API
  slug: zero-networks-ae-exclusions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-ae-exclusions-api-openapi.yml
- filename: zero-networks-assets-api-openapi.yml
  format: yaml
  label: Zero Networks Assets API
  slug: zero-networks-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-assets-api-openapi.yml
- filename: zero-networks-groups-custom-api-openapi.yml
  format: yaml
  label: Zero Networks Groups Custom API
  slug: zero-networks-groups-custom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-groups-custom-api-openapi.yml
- filename: zero-networks-internal-access-policy-api-openapi.yml
  format: yaml
  label: Zero Networks Internal Access Policy API
  slug: zero-networks-internal-access-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-internal-access-policy-api-openapi.yml
- filename: zero-networks-mfa-inbound-api-openapi.yml
  format: yaml
  label: Zero Networks MFA Inbound API
  slug: zero-networks-mfa-inbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-mfa-inbound-api-openapi.yml
- filename: zero-networks-mfa-outbound-api-openapi.yml
  format: yaml
  label: Zero Networks MFA Outbound API
  slug: zero-networks-mfa-outbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-mfa-outbound-api-openapi.yml
- filename: zero-networks-rules-inbound-api-openapi.yml
  format: yaml
  label: Zero Networks Rules Inbound API
  slug: zero-networks-rules-inbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-rules-inbound-api-openapi.yml
- filename: zero-networks-rules-outbound-api-openapi.yml
  format: yaml
  label: Zero Networks Rules Outbound API
  slug: zero-networks-rules-outbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-rules-outbound-api-openapi.yml
- filename: zero-networks-rules-rpc-api-openapi.yml
  format: yaml
  label: Zero Networks Rules RPC API
  slug: zero-networks-rules-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/openapi/zero-networks-rules-rpc-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Zero Networks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zero Networks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zero Networks
provider_slug: zero-networks
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/zero-networks-platform-openapi.yaml
  type: apiKey
slug: zero-networks-authentication
source_filename: zero-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/zero-networks-platform-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/zero-networks-platform-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zero-networks/refs/heads/main/authentication/zero-networks-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Network Security
- Microsegmentation
- Zero Trust
- Identity
- Multi-Factor Authentication
- Segmentation
- ZTNA
- Kubernetes
- Cybersecurity
---
