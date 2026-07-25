---
api_key_in:
- header
api_specs:
- filename: aws-security-hub-action-targets-api-openapi.yml
  format: yaml
  label: AWS Security Hub Action Targets API
  slug: aws-security-hub-action-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-action-targets-api-openapi.yml
- filename: aws-security-hub-automation-rules-api-openapi.yml
  format: yaml
  label: AWS Security Hub Automation Rules API
  slug: aws-security-hub-automation-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-automation-rules-api-openapi.yml
- filename: aws-security-hub-configuration-policies-api-openapi.yml
  format: yaml
  label: AWS Security Hub Configuration Policies API
  slug: aws-security-hub-configuration-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-configuration-policies-api-openapi.yml
- filename: aws-security-hub-controls-api-openapi.yml
  format: yaml
  label: AWS Security Hub Controls API
  slug: aws-security-hub-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-controls-api-openapi.yml
- filename: aws-security-hub-findings-api-openapi.yml
  format: yaml
  label: AWS Security Hub Findings API
  slug: aws-security-hub-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-findings-api-openapi.yml
- filename: aws-security-hub-hub-api-openapi.yml
  format: yaml
  label: AWS Security Hub Hub API
  slug: aws-security-hub-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-hub-api-openapi.yml
- filename: aws-security-hub-insights-api-openapi.yml
  format: yaml
  label: AWS Security Hub Insights API
  slug: aws-security-hub-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-insights-api-openapi.yml
- filename: aws-security-hub-invitations-api-openapi.yml
  format: yaml
  label: AWS Security Hub Invitations API
  slug: aws-security-hub-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-invitations-api-openapi.yml
- filename: aws-security-hub-members-api-openapi.yml
  format: yaml
  label: AWS Security Hub Members API
  slug: aws-security-hub-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-members-api-openapi.yml
- filename: aws-security-hub-standards-api-openapi.yml
  format: yaml
  label: AWS Security Hub Standards API
  slug: aws-security-hub-standards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-standards-api-openapi.yml
- filename: aws-security-hub-tags-api-openapi.yml
  format: yaml
  label: AWS Security Hub Tags API
  slug: aws-security-hub-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Security Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS Security Hub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS Security Hub
provider_slug: aws-security-hub
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed Authorization header
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/aws-security-hub-openapi.yml
  type: apiKey
slug: aws-security-hub-authentication
source_filename: aws-security-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-security-hub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed Authorization header\n  sources:\n  - openapi/aws-security-hub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/authentication/aws-security-hub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Cloud Security Posture Management
- Compliance
- Findings
- Threat Detection
- Cloud
---
