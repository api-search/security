---
api_key_in:
- header
api_specs:
- filename: amazon-well-architected-tool-consolidatedreport-format-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool ConsolidatedReport#Format API
  slug: amazon-well-architected-tool-consolidatedreport-format-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-consolidatedreport-format-api-openapi.yml
- filename: amazon-well-architected-tool-global-settings-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool Global Settings API
  slug: amazon-well-architected-tool-global-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-global-settings-api-openapi.yml
- filename: amazon-well-architected-tool-importlens-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool ImportLens API
  slug: amazon-well-architected-tool-importlens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-importlens-api-openapi.yml
- filename: amazon-well-architected-tool-lenses-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool Lenses API
  slug: amazon-well-architected-tool-lenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-lenses-api-openapi.yml
- filename: amazon-well-architected-tool-notifications-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool Notifications API
  slug: amazon-well-architected-tool-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-notifications-api-openapi.yml
- filename: amazon-well-architected-tool-profilenotifications-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool ProfileNotifications API
  slug: amazon-well-architected-tool-profilenotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-profilenotifications-api-openapi.yml
- filename: amazon-well-architected-tool-profiles-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool Profiles API
  slug: amazon-well-architected-tool-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-profiles-api-openapi.yml
- filename: amazon-well-architected-tool-profilesummaries-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool ProfileSummaries API
  slug: amazon-well-architected-tool-profilesummaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-profilesummaries-api-openapi.yml
- filename: amazon-well-architected-tool-profiletemplate-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool ProfileTemplate API
  slug: amazon-well-architected-tool-profiletemplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-profiletemplate-api-openapi.yml
- filename: amazon-well-architected-tool-shareinvitations-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool ShareInvitations API
  slug: amazon-well-architected-tool-shareinvitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-shareinvitations-api-openapi.yml
- filename: amazon-well-architected-tool-tags-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool Tags API
  slug: amazon-well-architected-tool-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-tags-api-openapi.yml
- filename: amazon-well-architected-tool-workloads-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool Workloads API
  slug: amazon-well-architected-tool-workloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-workloads-api-openapi.yml
- filename: amazon-well-architected-tool-workloadssummaries-api-openapi.yml
  format: yaml
  label: Amazon Well-Architected Tool WorkloadsSummaries API
  slug: amazon-well-architected-tool-workloadssummaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/openapi/amazon-well-architected-tool-workloadssummaries-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Well Architected Tool Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Well-Architected Tool secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-well-architected-tool-openapi-original.yaml
  type: apiKey
slug: amazon-well-architected-tool-authentication
source_filename: amazon-well-architected-tool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-well-architected-tool-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-well-architected-tool-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/authentication/amazon-well-architected-tool-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
---
