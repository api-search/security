---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Epicor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epicor declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Epicor
provider_slug: epicor
scheme_count: 1
schemes:
- description: API keys, access scopes, and standard authentication methods control which services and methods are available to each integration. Security aligns with existing ERP user and data permissions.
  type: apiKey
slug: epicor-authentication
source_filename: epicor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Epicor authentication\ngenerated: '2026-10-20'\nmethod: searched\nsource: https://www.epicor.com/en/products/enterprise-resource-planning-erp/epicor-kinetic/tools-and-technology/open-rest-api/\ndocs: https://www.epicor.com/en/products/enterprise-resource-planning-erp/epicor-kinetic/tools-and-technology/open-rest-api/\nschemes:\n  - type: apiKey\n    description: \"API keys, access scopes, and standard authentication methods control which services and methods are available to each integration. Security aligns with existing ERP user and data permissions.\"\nnote: Header names and key formats are documented only in the per-tenant Kinetic REST help, which is customer-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epicor/refs/heads/main/authentication/epicor-authentication.yml
summary_line: 1 scheme
tags:
- ERP
- Manufacturing
- Distribution
- Enterprise
- REST
- Fortune 500
---
