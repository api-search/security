---
api_key_in:
- cookie
- header
api_specs:
- filename: bonitasoft-bonita-openapi.yml
  format: yaml
  label: Bonita Web REST API
  slug: bonitasoft-bonita-web-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonitasoft/refs/heads/main/openapi/bonitasoft-bonita-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bonitasoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bonitasoft secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bonitasoft
provider_slug: bonitasoft
scheme_count: 3
schemes:
- description: To call the REST API, you must first log on with a user registered in the Engine database. Please refer to the __[Login API](#operation/login)__ operations section.
  in: cookie
  name: bonita_auth
  parameter: JSESSIONID
  sources:
  - openapi/bonitasoft-bonita-openapi.yml
  type: apiKey
- description: To call the REST API, you must first log on with a user registered in the Engine database. Please refer to the __[Login API](#operation/login)__ operations section.
  in: header
  name: bonita_token
  parameter: X-Bonita-API-Token
  sources:
  - openapi/bonitasoft-bonita-openapi.yml
  type: apiKey
- description: '![edition](https://img.shields.io/badge/edition-entreprise-blue)


    When Bonita runtime is configured for SSO with openID Connect it is possible To call the REST API directly with a Bearer Authorization header containing the access token.'
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/bonitasoft-bonita-openapi.yml
  type: http
slug: bonitasoft-authentication
source_filename: bonitasoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: derived\nsource: openapi/bonitasoft-bonita-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: bonita_auth\n  type: apiKey\n  in: cookie\n  parameter: JSESSIONID\n  description: To call the REST API, you must first log on with a user registered in the Engine\n    database. Please refer to the __[Login API](#operation/login)__ operations section.\n  sources:\n  - openapi/bonitasoft-bonita-openapi.yml\n- name: bonita_token\n  type: apiKey\n  in: header\n  parameter: X-Bonita-API-Token\n  description: To call the REST API, you must first log on with a user registered in the Engine\n    database. Please refer to the __[Login API](#operation/login)__ operations section.\n  sources:\n  - openapi/bonitasoft-bonita-openapi.yml\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  description: |-\n    ![edition](https://img.shields.io/badge/edition-entreprise-blue)\n\n    When Bonita runtime\
  \ is configured for SSO with openID Connect it is possible To call the REST API directly with a Bearer Authorization header containing the access token.\n  sources:\n  - openapi/bonitasoft-bonita-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonitasoft/refs/heads/main/authentication/bonitasoft-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Software-as-a-Service
- Business Process Management
- Process Automation
- Workflows
- BPMN
- Low-Code
- Open-Source
- Orchestration
- Agentic AI
- Case Management
- Java
---
