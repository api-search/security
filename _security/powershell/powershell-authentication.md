---
api_key_in:
- header
api_specs:
- filename: powershell-openapi.yml
  format: yaml
  label: PowerShell Gallery API
  slug: powershell-gallery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershell/refs/heads/main/openapi/powershell-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Powershell Authentication
name_suffix: Authentication
oauth_flows: []
overview: PowerShell secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PowerShell
provider_slug: powershell
scheme_count: 1
schemes:
- description: 'PowerShell Gallery publishing API key, issued from a signed-in PowerShell

    Gallery user account. Required for package push and unlist operations.'
  in: header
  name: galleryApiKey
  parameter: X-NuGet-ApiKey
  sources:
  - openapi/powershell-openapi.yml
  type: apiKey
slug: powershell-authentication
source_filename: powershell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/powershell-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: galleryApiKey\n  type: apiKey\n  in: header\n  parameter: X-NuGet-ApiKey\n  description: |-\n    PowerShell Gallery publishing API key, issued from a signed-in PowerShell\n    Gallery user account. Required for package push and unlist operations.\n  sources:\n  - openapi/powershell-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powershell/refs/heads/main/authentication/powershell-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- Command-Line
- Cross-Platform
- Scripting
- Shell
- Windows
- DevOps
---
