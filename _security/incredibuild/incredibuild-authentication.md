---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Incredibuild Authentication
name_suffix: Authentication
oauth_flows: []
overview: Incredibuild secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Incredibuild
provider_slug: incredibuild
scheme_count: 1
schemes:
- description: Custom API key sent in the client-api-key HTTPS request header. The key is created and copied from the Coordinator API configuration; the Coordinator must have Build Group APIs enabled and an API port configured (default 31100).
  in: header
  name: clientApiKey
  parameter_name: client-api-key
  source: https://docs.incredibuild.com/win/latest/windows/api.html
  type: apiKey
slug: incredibuild-authentication
source_filename: incredibuild-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.incredibuild.com/win/latest/windows/api.html\ndocs: https://docs.incredibuild.com/win/v9/windows/setting_up_API_environment.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: 'Incredibuild Build Group and Build History REST APIs authenticate with a\n    custom API key. The key is generated in the Coordinator and passed in every request\n    as an HTTPS header. There is no OpenAPI/Swagger definition published; this profile\n    is captured from the developer documentation.'\nschemes:\n- name: clientApiKey\n  type: apiKey\n  in: header\n  parameter_name: client-api-key\n  description: 'Custom API key sent in the client-api-key HTTPS request header. The\n    key is created and copied from the Coordinator API configuration; the Coordinator\n    must have Build Group APIs enabled and an API port configured (default 31100).'\n  source: https://docs.incredibuild.com/win/latest/windows/api.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incredibuild/refs/heads/main/authentication/incredibuild-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- DevOps
- Build Acceleration
- Continuous Integration
- Distributed Computing
- Build Cache
- Developer Tools
- CI/CD
---
