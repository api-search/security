---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft .NET secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft .NET
provider_slug: microsoft-net
scheme_count: 1
schemes:
- description: NuGet API key (required only for PackagePublish push/delete operations).
  in: header
  name: apiKey
  parameter: X-NuGet-ApiKey
  sources:
  - openapi/microsoft-net-openapi.yml
  type: apiKey
slug: microsoft-net-authentication
source_filename: microsoft-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-net-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-NuGet-ApiKey\n  description: NuGet API key (required only for PackagePublish push/delete operations).\n  sources:\n  - openapi/microsoft-net-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-net/refs/heads/main/authentication/microsoft-net-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- .NET
- C#
- Cloud
- Cross-Platform
- Developer Tools
- Microsoft
- Open Source
---
