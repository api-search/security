---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: caliuapp-com-api-keys-api-openapi.yml
  format: yaml
  label: Caliu API Keys API
  slug: caliuapp-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caliuapp-com/openapi/caliuapp-com-api-keys-api-openapi.yml
- filename: caliuapp-com-attachments-api-openapi.yml
  format: yaml
  label: Caliu Attachments API
  slug: caliuapp-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caliuapp-com/openapi/caliuapp-com-attachments-api-openapi.yml
- filename: caliuapp-com-auth-api-openapi.yml
  format: yaml
  label: Caliu Auth API
  slug: caliuapp-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caliuapp-com/openapi/caliuapp-com-auth-api-openapi.yml
- filename: caliuapp-com-devices-api-openapi.yml
  format: yaml
  label: Caliu Devices API
  slug: caliuapp-com-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caliuapp-com/openapi/caliuapp-com-devices-api-openapi.yml
- filename: caliuapp-com-export-api-openapi.yml
  format: yaml
  label: Caliu Export API
  slug: caliuapp-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caliuapp-com/openapi/caliuapp-com-export-api-openapi.yml
- filename: caliuapp-com-notes-api-openapi.yml
  format: yaml
  label: Caliu Notes API
  slug: caliuapp-com-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caliuapp-com/openapi/caliuapp-com-notes-api-openapi.yml
- filename: caliuapp-com-reminders-api-openapi.yml
  format: yaml
  label: Caliu Reminders API
  slug: caliuapp-com-reminders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caliuapp-com/openapi/caliuapp-com-reminders-api-openapi.yml
- filename: caliuapp-com-subscription-api-openapi.yml
  format: yaml
  label: Caliu Subscription API
  slug: caliuapp-com-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caliuapp-com/openapi/caliuapp-com-subscription-api-openapi.yml
- filename: caliuapp-com-tags-api-openapi.yml
  format: yaml
  label: Caliu Tags API
  slug: caliuapp-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caliuapp-com/openapi/caliuapp-com-tags-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Caliuapp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Caliu secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Caliu
provider_slug: caliuapp-com
scheme_count: 2
schemes:
- description: API key (caliu_xxx) or session token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/caliuapp-com-openapi.json
  type: http
- in: cookie
  name: cookieAuth
  parameter: caliu_session
  sources:
  - openapi/caliuapp-com-openapi.json
  type: apiKey
slug: caliuapp-com-authentication
source_filename: caliuapp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/caliuapp-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key (caliu_xxx) or session token\n  sources:\n  - openapi/caliuapp-com-openapi.json\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: caliu_session\n  sources:\n  - openapi/caliuapp-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/caliuapp-com/authentication/caliuapp-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Note Taking
- Privacy
- Local-First
- Markdown
- Cross-Platform
---
