---
api_key_in:
- header
api_specs:
- filename: appian-openapi.yml
  format: yaml
  label: Appian Application Package Details API
  slug: appian
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/openapi/appian-openapi.yml
- filename: appian-deployment-rest-openapi.yml
  format: yaml
  label: Appian Deployment REST API
  slug: deployment-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/openapi/appian-deployment-rest-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Appian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appian secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appian
provider_slug: appian
scheme_count: 1
schemes:
- description: API key linked to a service account. Created and managed through the Appian Admin Console. The service account must have access to the application via the application's role map.
  in: header
  name: apiKeyAuth
  parameter: appian-api-key
  sources:
  - openapi/appian-application-package-details-openapi.yml
  - openapi/appian-deployment-rest-openapi.yml
  type: apiKey
slug: appian-authentication
source_filename: appian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appian-application-package-details-openapi.yml, openapi/appian-deployment-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: appian-api-key\n  description: API key linked to a service account. Created and managed through the Appian Admin\n    Console. The service account must have access to the application via the application's role\n    map.\n  sources:\n  - openapi/appian-application-package-details-openapi.yml\n  - openapi/appian-deployment-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/authentication/appian-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
---
