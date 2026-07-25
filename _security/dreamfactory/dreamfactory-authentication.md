---
api_key_in:
- header
api_specs:
- filename: dreamfactory-system-api-openapi.yml
  format: yaml
  label: DreamFactory System API
  slug: system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-system-api-openapi.yml
- filename: dreamfactory-admin-api-openapi.yml
  format: yaml
  label: DreamFactory Admin API
  slug: dreamfactory-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-admin-api-openapi.yml
- filename: dreamfactory-app-api-openapi.yml
  format: yaml
  label: DreamFactory App API
  slug: dreamfactory-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-app-api-openapi.yml
- filename: dreamfactory-appgroup-api-openapi.yml
  format: yaml
  label: DreamFactory AppGroup API
  slug: dreamfactory-appgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-appgroup-api-openapi.yml
- filename: dreamfactory-cors-api-openapi.yml
  format: yaml
  label: DreamFactory CORS API
  slug: dreamfactory-cors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-cors-api-openapi.yml
- filename: dreamfactory-custom-api-openapi.yml
  format: yaml
  label: DreamFactory Custom API
  slug: dreamfactory-custom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-custom-api-openapi.yml
- filename: dreamfactory-emailtemplate-api-openapi.yml
  format: yaml
  label: DreamFactory EmailTemplate API
  slug: dreamfactory-emailtemplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-emailtemplate-api-openapi.yml
- filename: dreamfactory-environment-api-openapi.yml
  format: yaml
  label: DreamFactory Environment API
  slug: dreamfactory-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-environment-api-openapi.yml
- filename: dreamfactory-event-api-openapi.yml
  format: yaml
  label: DreamFactory Event API
  slug: dreamfactory-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-event-api-openapi.yml
- filename: dreamfactory-limit-api-openapi.yml
  format: yaml
  label: DreamFactory Limit API
  slug: dreamfactory-limit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-limit-api-openapi.yml
- filename: dreamfactory-lookup-api-openapi.yml
  format: yaml
  label: DreamFactory Lookup API
  slug: dreamfactory-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-lookup-api-openapi.yml
- filename: dreamfactory-package-api-openapi.yml
  format: yaml
  label: DreamFactory Package API
  slug: dreamfactory-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-package-api-openapi.yml
- filename: dreamfactory-role-api-openapi.yml
  format: yaml
  label: DreamFactory Role API
  slug: dreamfactory-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-role-api-openapi.yml
- filename: dreamfactory-scripttype-api-openapi.yml
  format: yaml
  label: DreamFactory ScriptType API
  slug: dreamfactory-scripttype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-scripttype-api-openapi.yml
- filename: dreamfactory-servicetype-api-openapi.yml
  format: yaml
  label: DreamFactory ServiceType API
  slug: dreamfactory-servicetype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-servicetype-api-openapi.yml
- filename: dreamfactory-user-api-openapi.yml
  format: yaml
  label: DreamFactory User API
  slug: dreamfactory-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/openapi/dreamfactory-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dreamfactory Authentication
name_suffix: Authentication
oauth_flows: []
overview: DreamFactory secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DreamFactory
provider_slug: dreamfactory
scheme_count: 2
schemes:
- description: Session token obtained after admin login.
  in: header
  name: sessionToken
  parameter: X-DreamFactory-Session-Token
  sources:
  - openapi/dreamfactory-system-api-openapi.yml
  type: apiKey
- description: API key associated with a registered application.
  in: header
  name: apiKey
  parameter: X-DreamFactory-API-Key
  sources:
  - openapi/dreamfactory-system-api-openapi.yml
  type: apiKey
slug: dreamfactory-authentication
source_filename: dreamfactory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dreamfactory-system-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: X-DreamFactory-Session-Token\n  description: Session token obtained after admin login.\n  sources:\n  - openapi/dreamfactory-system-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-DreamFactory-API-Key\n  description: API key associated with a registered application.\n  sources:\n  - openapi/dreamfactory-system-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dreamfactory/refs/heads/main/authentication/dreamfactory-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Automation
- Deployment
- Documentation
- Generation
- Security
---
