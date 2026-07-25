---
api_key_in: []
api_specs:
- filename: fullstory-sessions-api-openapi.yml
  format: yaml
  label: FullStory Sessions API
  slug: fullstory-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-sessions-api-openapi.yml
- filename: fullstory-batch-import-api-openapi.yml
  format: yaml
  label: FullStory Batch Import API
  slug: fullstory-batch-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-batch-import-api-openapi.yml
- filename: fullstory-endpoints-api-openapi.yml
  format: yaml
  label: FullStory Endpoints API
  slug: fullstory-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-endpoints-api-openapi.yml
- filename: fullstory-event-types-api-openapi.yml
  format: yaml
  label: FullStory Event Types API
  slug: fullstory-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-event-types-api-openapi.yml
- filename: fullstory-events-api-openapi.yml
  format: yaml
  label: FullStory Events API
  slug: fullstory-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-events-api-openapi.yml
- filename: fullstory-exports-api-openapi.yml
  format: yaml
  label: FullStory Exports API
  slug: fullstory-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-exports-api-openapi.yml
- filename: fullstory-operations-api-openapi.yml
  format: yaml
  label: FullStory Operations API
  slug: fullstory-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-operations-api-openapi.yml
- filename: fullstory-segments-api-openapi.yml
  format: yaml
  label: FullStory Segments API
  slug: fullstory-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-segments-api-openapi.yml
- filename: fullstory-session-events-api-openapi.yml
  format: yaml
  label: FullStory Session Events API
  slug: fullstory-session-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-session-events-api-openapi.yml
- filename: fullstory-session-summaries-api-openapi.yml
  format: yaml
  label: FullStory Session Summaries API
  slug: fullstory-session-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-session-summaries-api-openapi.yml
- filename: fullstory-users-api-openapi.yml
  format: yaml
  label: FullStory Users API
  slug: fullstory-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-users-api-openapi.yml
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
