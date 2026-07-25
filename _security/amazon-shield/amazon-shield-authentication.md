---
api_key_in:
- header
api_specs:
- filename: amazon-shield-amazon-shield-rest-api-api-openapi.yml
  format: yaml
  label: Amazon Shield Amazon Shield REST API API
  slug: amazon-shield-amazon-shield-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/openapi/amazon-shield-amazon-shield-rest-api-api-openapi.yml
- filename: amazon-shield-createprotectiongroup-api-openapi.yml
  format: yaml
  label: 'Amazon Shield #CreateProtectionGroup API'
  slug: amazon-shield-createprotectiongroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/openapi/amazon-shield-createprotectiongroup-api-openapi.yml
- filename: amazon-shield-createsubscription-api-openapi.yml
  format: yaml
  label: 'Amazon Shield #CreateSubscription API'
  slug: amazon-shield-createsubscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/openapi/amazon-shield-createsubscription-api-openapi.yml
- filename: amazon-shield-describeattack-api-openapi.yml
  format: yaml
  label: 'Amazon Shield #DescribeAttack API'
  slug: amazon-shield-describeattack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/openapi/amazon-shield-describeattack-api-openapi.yml
- filename: amazon-shield-describeprotection-api-openapi.yml
  format: yaml
  label: 'Amazon Shield #DescribeProtection API'
  slug: amazon-shield-describeprotection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/openapi/amazon-shield-describeprotection-api-openapi.yml
- filename: amazon-shield-describesubscription-api-openapi.yml
  format: yaml
  label: 'Amazon Shield #DescribeSubscription API'
  slug: amazon-shield-describesubscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/openapi/amazon-shield-describesubscription-api-openapi.yml
- filename: amazon-shield-listprotections-api-openapi.yml
  format: yaml
  label: 'Amazon Shield #ListProtections API'
  slug: amazon-shield-listprotections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/openapi/amazon-shield-listprotections-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Shield Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Shield secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Shield
provider_slug: amazon-shield
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-shield-api-openapi.yml
  type: apiKey
slug: amazon-shield-authentication
source_filename: amazon-shield-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-shield-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-shield-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/authentication/amazon-shield-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DDoS Protection
- Networking
- Security
---
