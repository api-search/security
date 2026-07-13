---
api_key_in:
- header
api_specs:
- filename: web-of-science-starter-openapi.yml
  format: yaml
  label: Web of Science Starter API
  slug: web-of-science-starter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/web-of-science-apis/refs/heads/main/openapi/web-of-science-starter-openapi.yml
- filename: web-of-science-expanded-openapi.yml
  format: yaml
  label: Web of Science API Expanded
  slug: web-of-science-expanded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/web-of-science-apis/refs/heads/main/openapi/web-of-science-expanded-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Web Of Science Apis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Web of Science APIs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Web of Science APIs
provider_slug: web-of-science-apis
scheme_count: 1
schemes:
- description: Clarivate API key for Web of Science API Expanded
  in: header
  name: ApiKeyAuth
  parameter: X-ApiKey
  sources:
  - openapi/web-of-science-expanded-openapi.yml
  - openapi/web-of-science-starter-openapi.yml
  type: apiKey
slug: web-of-science-apis-authentication
source_filename: web-of-science-apis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/web-of-science-expanded-openapi.yml, openapi/web-of-science-starter-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-ApiKey\n  description: Clarivate API key for Web of Science API Expanded\n  sources:\n  - openapi/web-of-science-expanded-openapi.yml\n  - openapi/web-of-science-starter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/web-of-science-apis/refs/heads/main/authentication/web-of-science-apis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Research
- Academic
- Bibliometrics
- Citations
- Science
- Scholarly
---
