---
api_key_in:
- header
api_specs:
- filename: microsoft-nuget-openapi.yml
  format: yaml
  label: NuGet Server API
  slug: server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-nuget/refs/heads/main/openapi/microsoft-nuget-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Nuget Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft NuGet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft NuGet
provider_slug: microsoft-nuget
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-NuGet-ApiKey
  sources:
  - openapi/microsoft-nuget-openapi.yml
  type: apiKey
slug: microsoft-nuget-authentication
source_filename: microsoft-nuget-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-nuget-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-NuGet-ApiKey\n  sources:\n  - openapi/microsoft-nuget-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-nuget/refs/heads/main/authentication/microsoft-nuget-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- .NET
- Microsoft
- NuGet
- Package Management
---
