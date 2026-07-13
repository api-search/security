---
api_key_in: []
api_specs:
- filename: iis-administration-api.yml
  format: yaml
  label: IIS Administration API
  slug: iis-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/openapi/iis-administration-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Windows Server Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Windows Server secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
scheme_count: 1
schemes:
- description: Access token for authenticating with the IIS Administration API. Tokens are generated through the API management portal at https://localhost:55539.
  name: accessToken
  scheme: bearer
  sources:
  - openapi/iis-administration-api.yml
  type: http
slug: microsoft-windows-server-authentication
source_filename: microsoft-windows-server-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/iis-administration-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessToken\n  type: http\n  scheme: bearer\n  description: Access token for authenticating with the IIS Administration API. Tokens are generated\n    through the API management portal at https://localhost:55539.\n  sources:\n  - openapi/iis-administration-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/authentication/microsoft-windows-server-authentication.yml
summary_line: http · 1 scheme
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
---
