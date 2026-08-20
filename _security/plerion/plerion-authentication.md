---
api_key_in: []
api_specs:
- filename: plerion-alerts-api-openapi.yml
  format: yaml
  label: Plerion Alerts API
  slug: plerion-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-alerts-api-openapi.yml
- filename: plerion-asset-groups-api-openapi.yml
  format: yaml
  label: Plerion Asset groups API
  slug: plerion-asset-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-asset-groups-api-openapi.yml
- filename: plerion-assets-api-openapi.yml
  format: yaml
  label: Plerion Assets API
  slug: plerion-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-assets-api-openapi.yml
- filename: plerion-audit-logs-api-openapi.yml
  format: yaml
  label: Plerion Audit logs API
  slug: plerion-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-audit-logs-api-openapi.yml
- filename: plerion-aws-integration-api-openapi.yml
  format: yaml
  label: Plerion AWS integration API
  slug: plerion-aws-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-aws-integration-api-openapi.yml
- filename: plerion-code-security-api-openapi.yml
  format: yaml
  label: Plerion Code security API
  slug: plerion-code-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-code-security-api-openapi.yml
- filename: plerion-compliance-frameworks-api-openapi.yml
  format: yaml
  label: Plerion Compliance frameworks API
  slug: plerion-compliance-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-compliance-frameworks-api-openapi.yml
- filename: plerion-findings-api-openapi.yml
  format: yaml
  label: Plerion Findings API
  slug: plerion-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-findings-api-openapi.yml
- filename: plerion-integrations-api-openapi.yml
  format: yaml
  label: Plerion Integrations API
  slug: plerion-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-integrations-api-openapi.yml
- filename: plerion-risks-api-openapi.yml
  format: yaml
  label: Plerion Risks API
  slug: plerion-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-risks-api-openapi.yml
- filename: plerion-tenant-api-openapi.yml
  format: yaml
  label: Plerion Tenant API
  slug: plerion-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-tenant-api-openapi.yml
- filename: plerion-vulnerabilities-api-openapi.yml
  format: yaml
  label: Plerion Vulnerabilities API
  slug: plerion-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-vulnerabilities-api-openapi.yml
- filename: plerion-well-architected-frameworks-api-openapi.yml
  format: yaml
  label: Plerion Well-Architected frameworks API
  slug: plerion-well-architected-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/openapi/plerion-well-architected-frameworks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Plerion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plerion secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plerion
provider_slug: plerion
scheme_count: 1
schemes:
- bearerFormat: apiKey
  description: Bearer API Key. For example, "Bearer {Tenant API Key}"
  docs: https://docs.plerion.com/api-reference/index
  key_management: https://app.plerion.com/settings/api-keys
  name: APIKey
  scheme: bearer
  sources:
  - openapi/plerion-openapi-original.yml
  type: http
slug: plerion-authentication
source_filename: plerion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/plerion-openapi-original.yml\ndocs: https://docs.plerion.com/api-reference/index\nkey_management: https://app.plerion.com/settings/api-keys\nsummary:\n  types:\n  - http\n  model: Tenant API Key sent as an HTTP Bearer token\n  header: 'Authorization: Bearer $PLERION_API_KEY'\n  transport: HTTPS required (plain HTTP requests fail)\nschemes:\n- name: APIKey\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  description: Bearer API Key. For example, \"Bearer {Tenant API Key}\"\n  docs: https://docs.plerion.com/api-reference/index\n  key_management: https://app.plerion.com/settings/api-keys\n  sources:\n  - openapi/plerion-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plerion/refs/heads/main/authentication/plerion-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cloud Security
- CSPM
- Cloud Workload Protection
- Vulnerability Management
- Compliance
- AI Security
- DevSecOps
---
