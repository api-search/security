---
api_key_in:
- header
api_specs:
- filename: free-law-project-alerts-api-openapi.yml
  format: yaml
  label: Free Law Project Alerts API
  slug: free-law-project-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-alerts-api-openapi.yml
- filename: free-law-project-case-law-api-openapi.yml
  format: yaml
  label: Free Law Project Case Law API
  slug: free-law-project-case-law-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-case-law-api-openapi.yml
- filename: free-law-project-citations-api-openapi.yml
  format: yaml
  label: Free Law Project Citations API
  slug: free-law-project-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-citations-api-openapi.yml
- filename: free-law-project-financial-disclosures-api-openapi.yml
  format: yaml
  label: Free Law Project Financial Disclosures API
  slug: free-law-project-financial-disclosures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-financial-disclosures-api-openapi.yml
- filename: free-law-project-judges-api-openapi.yml
  format: yaml
  label: Free Law Project Judges API
  slug: free-law-project-judges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-judges-api-openapi.yml
- filename: free-law-project-oral-arguments-api-openapi.yml
  format: yaml
  label: Free Law Project Oral Arguments API
  slug: free-law-project-oral-arguments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-oral-arguments-api-openapi.yml
- filename: free-law-project-pacer-api-openapi.yml
  format: yaml
  label: Free Law Project PACER API
  slug: free-law-project-pacer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-pacer-api-openapi.yml
- filename: free-law-project-recap-api-openapi.yml
  format: yaml
  label: Free Law Project RECAP API
  slug: free-law-project-recap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-recap-api-openapi.yml
- filename: free-law-project-search-api-openapi.yml
  format: yaml
  label: Free Law Project Search API
  slug: free-law-project-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-search-api-openapi.yml
- filename: free-law-project-tags-api-openapi.yml
  format: yaml
  label: Free Law Project Tags API
  slug: free-law-project-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Free Law Project Authentication
name_suffix: Authentication
oauth_flows: []
overview: Free Law Project secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Free Law Project
provider_slug: free-law-project
scheme_count: 1
schemes:
- description: 'HTTP token authentication. Format: `Token <your-token>`.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/free-law-project-openapi.yml
  type: apiKey
slug: free-law-project-authentication
source_filename: free-law-project-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/free-law-project-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'HTTP token authentication. Format: `Token <your-token>`.'\n  sources:\n  - openapi/free-law-project-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/authentication/free-law-project-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Courts
- Justice
- Legal
- Transparency
---
