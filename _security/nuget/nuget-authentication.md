---
api_key_in:
- header
api_specs:
- filename: nuget-server-api-openapi.yml
  format: yaml
  label: NuGet Server API
  slug: nuget-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-server-api-openapi.yml
- filename: nuget-catalog-api-openapi.yml
  format: yaml
  label: NuGet Catalog API
  slug: nuget-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-catalog-api-openapi.yml
- filename: nuget-search-api-openapi.yml
  format: yaml
  label: NuGet Search API
  slug: nuget-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-search-api-openapi.yml
- filename: nuget-package-metadata-api-openapi.yml
  format: yaml
  label: NuGet Package Metadata API
  slug: nuget-package-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-package-metadata-api-openapi.yml
- filename: nuget-package-content-api-openapi.yml
  format: yaml
  label: NuGet Package Content API
  slug: nuget-package-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-package-content-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nuget Authentication
name_suffix: Authentication
oauth_flows: []
overview: NuGet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NuGet
provider_slug: nuget
scheme_count: 1
schemes:
- description: An API key obtained from the NuGet package source. Required for push, delete, and relist operations.
  in: header
  name: apiKey
  parameter: X-NuGet-ApiKey
  sources:
  - openapi/nuget-server-api-openapi.yml
  type: apiKey
slug: nuget-authentication
source_filename: nuget-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nuget-server-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-NuGet-ApiKey\n  description: An API key obtained from the NuGet package source. Required for push, delete,\n    and relist operations.\n  sources:\n  - openapi/nuget-server-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/authentication/nuget-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Package Management
- .NET
- Packages
- Dependencies
- Software Distribution
- Registry
---
