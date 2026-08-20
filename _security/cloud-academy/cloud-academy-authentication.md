---
api_key_in: []
api_specs:
- filename: cloud-academy-learning-management-system-api-openapi.yml
  format: yaml
  label: Cloud Academy Learning Management System API
  slug: cloud-academy-learning-management-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-academy/refs/heads/main/openapi/cloud-academy-learning-management-system-api-openapi.yml
- filename: cloud-academy-organizations-api-openapi.yml
  format: yaml
  label: Cloud Academy Organizations API
  slug: cloud-academy-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-academy/refs/heads/main/openapi/cloud-academy-organizations-api-openapi.yml
- filename: cloud-academy-reports-api-openapi.yml
  format: yaml
  label: Cloud Academy Reports API
  slug: cloud-academy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-academy/refs/heads/main/openapi/cloud-academy-reports-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cloud Academy Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cloud Academy secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cloud Academy
provider_slug: cloud-academy
scheme_count: 1
schemes:
- description: Insert your API key pair.<br/><br/>Enterprise members with Admin permissions can generate and view their own API keys on the settings area of their Company Account [here](https://platform.qa.com/organizations/settings/api/).
  flows:
  - authorizationUrl: https://platform.qa.com/oauth2/authorize/
    flow: clientCredentials
    scopes: 0
    tokenUrl: https://platform.qa.com/oauth2/token/
  name: oauth2
  sources:
  - openapi/cloud-academy-openapi-original.json
  type: oauth2
slug: cloud-academy-authentication
source_filename: cloud-academy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cloud-academy-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    authorizationUrl: https://platform.qa.com/oauth2/authorize/\n    tokenUrl: https://platform.qa.com/oauth2/token/\n    scopes: 0\n  description: Insert your API key pair.<br/><br/>Enterprise members with Admin permissions\n    can generate and view their own API keys on the settings area of their Company Account [here](https://platform.qa.com/organizations/settings/api/).\n  sources:\n  - openapi/cloud-academy-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-academy/refs/heads/main/authentication/cloud-academy-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Training
- Education
- Learning Management
- Cloud Computing
- Skills
- Reporting
- E-Learning
---
