---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Package Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Package secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Package
provider_slug: microsoft-package
scheme_count: 1
schemes:
- description: Required only for publish/delete operations on nuget.org.
  in: header
  name: apiKey
  parameter: X-NuGet-ApiKey
  sources:
  - openapi/microsoft-package-openapi.yml
  type: apiKey
slug: microsoft-package-authentication
source_filename: microsoft-package-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-package-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-NuGet-ApiKey\n  description: Required only for publish/delete operations on nuget.org.\n  sources:\n  - openapi/microsoft-package-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-package/refs/heads/main/authentication/microsoft-package-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Azure Artifacts
- Microsoft
- NuGet
- Package Management
- WinGet
---
