---
api_key_in: []
api_specs:
- filename: fullstory-server-api-openapi.yml
  format: yaml
  label: FullStory Server API
  slug: fullstory-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-server-api-openapi.yml
- filename: fullstory-sessions-api-openapi.yml
  format: yaml
  label: FullStory Sessions API
  slug: fullstory-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-sessions-api-openapi.yml
- filename: fullstory-segments-export-api-openapi.yml
  format: yaml
  label: FullStory Segments Export API
  slug: fullstory-segments-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-segments-export-api-openapi.yml
- filename: fullstory-webhooks-api-openapi.yml
  format: yaml
  label: FullStory Webhooks API
  slug: fullstory-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fullstory Authentication
name_suffix: Authentication
oauth_flows: []
overview: FullStory secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FullStory
provider_slug: fullstory
scheme_count: 1
schemes:
- description: API key passed in the Authorization header using Basic authentication. Admin or Architect level keys are required.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fullstory-segments-export-api-openapi.yml
  - openapi/fullstory-server-api-openapi.yml
  - openapi/fullstory-sessions-api-openapi.yml
  - openapi/fullstory-webhooks-api-openapi.yml
  type: http
slug: fullstory-authentication
source_filename: fullstory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fullstory-segments-export-api-openapi.yml, openapi/fullstory-server-api-openapi.yml,\n  openapi/fullstory-sessions-api-openapi.yml, openapi/fullstory-webhooks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: API key passed in the Authorization header using Basic authentication. Admin\n    or Architect level keys are required.\n  sources:\n  - openapi/fullstory-segments-export-api-openapi.yml\n  - openapi/fullstory-server-api-openapi.yml\n  - openapi/fullstory-sessions-api-openapi.yml\n  - openapi/fullstory-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/authentication/fullstory-authentication.yml
summary_line: http · 1 scheme
tags:
- Session Replay
- Product Analytics
- Digital Experience
- Behavioral Analytics
- Frontend Monitoring
---
