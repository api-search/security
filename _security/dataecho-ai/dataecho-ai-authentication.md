---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dataecho-ai-analytics-api-openapi.yml
  format: yaml
  label: DataEcho Analytics API
  slug: dataecho-ai-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-analytics-api-openapi.yml
- filename: dataecho-ai-auth-api-openapi.yml
  format: yaml
  label: DataEcho Auth API
  slug: dataecho-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-auth-api-openapi.yml
- filename: dataecho-ai-domains-api-openapi.yml
  format: yaml
  label: DataEcho Domains API
  slug: dataecho-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-domains-api-openapi.yml
- filename: dataecho-ai-drives-api-openapi.yml
  format: yaml
  label: DataEcho Drives API
  slug: dataecho-ai-drives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-drives-api-openapi.yml
- filename: dataecho-ai-handles-api-openapi.yml
  format: yaml
  label: DataEcho Handles API
  slug: dataecho-ai-handles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-handles-api-openapi.yml
- filename: dataecho-ai-links-api-openapi.yml
  format: yaml
  label: DataEcho Links API
  slug: dataecho-ai-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-links-api-openapi.yml
- filename: dataecho-ai-profile-api-openapi.yml
  format: yaml
  label: DataEcho Profile API
  slug: dataecho-ai-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-profile-api-openapi.yml
- filename: dataecho-ai-site-data-api-openapi.yml
  format: yaml
  label: DataEcho Site Data API
  slug: dataecho-ai-site-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-site-data-api-openapi.yml
- filename: dataecho-ai-sites-api-openapi.yml
  format: yaml
  label: DataEcho Sites API
  slug: dataecho-ai-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-sites-api-openapi.yml
- filename: dataecho-ai-variables-api-openapi.yml
  format: yaml
  label: DataEcho Variables API
  slug: dataecho-ai-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataecho-ai/openapi/dataecho-ai-variables-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dataecho Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataEcho secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataEcho
provider_slug: dataecho-ai
scheme_count: 1
schemes:
- description: API key or drive token (drv_live_…) where noted.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dataecho-ai-openapi.yml
  type: http
slug: dataecho-ai-authentication
source_filename: dataecho-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/dataecho-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key or drive token (drv_live_…) where noted.\n  sources:\n  - openapi/dataecho-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dataecho-ai/authentication/dataecho-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Hosting
- Cloud Storage
- Free
---
