---
api_key_in:
- header
api_specs:
- filename: tenable-vulnerability-management-openapi.json
  format: json
  label: Tenable Vulnerability Management API
  slug: tenable-vulnerability-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-vulnerability-management-openapi.json
- filename: tenable-web-app-scanning-openapi.json
  format: json
  label: Tenable Web Application Scanning API
  slug: tenable-web-application-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-web-app-scanning-openapi.json
- filename: tenable-exposure-management-openapi.json
  format: json
  label: Tenable Exposure Management API
  slug: tenable-exposure-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-exposure-management-openapi.json
- filename: tenable-tenable-platform-settings-openapi.json
  format: json
  label: Tenable Platform & Settings API
  slug: tenable-platform-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-tenable-platform-settings-openapi.json
- filename: tenable-pci-asv-openapi.json
  format: json
  label: Tenable PCI ASV API
  slug: tenable-pci-asv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-pci-asv-openapi.json
- filename: tenable-mssp-openapi.json
  format: json
  label: Tenable MSSP Portal API
  slug: tenable-mssp-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-mssp-openapi.json
- filename: tenable-identity-exposure-openapi.json
  format: json
  label: Tenable Identity Exposure API
  slug: tenable-identity-exposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-identity-exposure-openapi.json
- filename: tenable-downloads-api-openapi.json
  format: json
  label: Tenable Downloads API
  slug: tenable-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-downloads-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tenable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tenable secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tenable
provider_slug: tenable
scheme_count: 3
schemes:
- description: 'Example: Bearer {{token}}'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/tenable-downloads-api-openapi.json
  type: apiKey
- description: Format - accessKey=ACCESS_KEY;secretKey=SECRET_KEY
  in: header
  name: Attack_Path_cloud
  parameter: X-ApiKeys
  sources:
  - openapi/tenable-exposure-management-openapi.json
  - openapi/tenable-mssp-openapi.json
  - openapi/tenable-pci-asv-openapi.json
  - openapi/tenable-tenable-platform-settings-openapi.json
  - openapi/tenable-vulnerability-management-openapi.json
  - openapi/tenable-web-app-scanning-openapi.json
  type: apiKey
- description: The user's API key
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/tenable-identity-exposure-openapi.json
  type: apiKey
slug: tenable-authentication
source_filename: tenable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://developer.tenable.com/docs/authorization\nsource: openapi/tenable-downloads-api-openapi.json, openapi/tenable-exposure-management-openapi.json,\n  openapi/tenable-identity-exposure-openapi.json, openapi/tenable-mssp-openapi.json, openapi/tenable-pci-asv-openapi.json,\n  openapi/tenable-tenable-platform-settings-openapi.json, openapi/tenable-vulnerability-management-openapi.json,\n  openapi/tenable-web-app-scanning-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Example: Bearer {{token}}'\n  sources:\n  - openapi/tenable-downloads-api-openapi.json\n- name: Attack_Path_cloud\n  type: apiKey\n  in: header\n  parameter: X-ApiKeys\n  description: Format - accessKey=ACCESS_KEY;secretKey=SECRET_KEY\n  sources:\n  - openapi/tenable-exposure-management-openapi.json\n  - openapi/tenable-mssp-openapi.json\n\
  \  - openapi/tenable-pci-asv-openapi.json\n  - openapi/tenable-tenable-platform-settings-openapi.json\n  - openapi/tenable-vulnerability-management-openapi.json\n  - openapi/tenable-web-app-scanning-openapi.json\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The user's API key\n  sources:\n  - openapi/tenable-identity-exposure-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/authentication/tenable-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Enterprise
- Cybersecurity
- Vulnerability Management
- Exposure Management
- Security
- Cloud Security
- Attack Surface Management
---
