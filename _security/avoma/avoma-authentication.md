---
anonymous_access: false
api_key_in: []
api_specs:
- filename: avoma-calls-api-openapi.yml
  format: yaml
  label: Avoma Calls API
  slug: avoma-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-calls-api-openapi.yml
- filename: avoma-custom-category-api-openapi.yml
  format: yaml
  label: Avoma Custom Category API
  slug: avoma-custom-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-custom-category-api-openapi.yml
- filename: avoma-engagement-analytics-api-openapi.yml
  format: yaml
  label: Avoma Engagement Analytics API
  slug: avoma-engagement-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-engagement-analytics-api-openapi.yml
- filename: avoma-meeting-outcomes-api-openapi.yml
  format: yaml
  label: Avoma Meeting Outcomes API
  slug: avoma-meeting-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meeting-outcomes-api-openapi.yml
- filename: avoma-meeting-types-api-openapi.yml
  format: yaml
  label: Avoma Meeting Types API
  slug: avoma-meeting-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meeting-types-api-openapi.yml
- filename: avoma-meetings-api-openapi.yml
  format: yaml
  label: Avoma Meetings API
  slug: avoma-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meetings-api-openapi.yml
- filename: avoma-meetings-sentiments-api-openapi.yml
  format: yaml
  label: Avoma Meetings Sentiments API
  slug: avoma-meetings-sentiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meetings-sentiments-api-openapi.yml
- filename: avoma-notes-api-openapi.yml
  format: yaml
  label: Avoma Notes API
  slug: avoma-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-notes-api-openapi.yml
- filename: avoma-recording-api-openapi.yml
  format: yaml
  label: Avoma Recording API
  slug: avoma-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-recording-api-openapi.yml
- filename: avoma-revenue-intelligence-beta-api-openapi.yml
  format: yaml
  label: Avoma Revenue Intelligence [Beta] API
  slug: avoma-revenue-intelligence-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-revenue-intelligence-beta-api-openapi.yml
- filename: avoma-scorecard-evaluations-api-openapi.yml
  format: yaml
  label: Avoma Scorecard Evaluations API
  slug: avoma-scorecard-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-scorecard-evaluations-api-openapi.yml
- filename: avoma-scorecards-api-openapi.yml
  format: yaml
  label: Avoma Scorecards API
  slug: avoma-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-scorecards-api-openapi.yml
- filename: avoma-smart-category-api-openapi.yml
  format: yaml
  label: Avoma Smart Category API
  slug: avoma-smart-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-smart-category-api-openapi.yml
- filename: avoma-snippets-api-openapi.yml
  format: yaml
  label: Avoma Snippets API
  slug: avoma-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-snippets-api-openapi.yml
- filename: avoma-templates-api-openapi.yml
  format: yaml
  label: Avoma Templates API
  slug: avoma-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-templates-api-openapi.yml
- filename: avoma-transcriptions-api-openapi.yml
  format: yaml
  label: Avoma Transcriptions API
  slug: avoma-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-transcriptions-api-openapi.yml
- filename: avoma-users-api-openapi.yml
  format: yaml
  label: Avoma Users API
  slug: avoma-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-users-api-openapi.yml
- filename: avoma-webhooks-api-openapi.yml
  format: yaml
  label: Avoma Webhooks API
  slug: avoma-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Avoma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avoma secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Avoma
provider_slug: avoma
scheme_count: 1
schemes:
- description: Avoma uses bearer token for authentication of the client. For now, you will have to contact [Avoma Support](mailto:help@avoma.com) to get one issued for you.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/avoma-openapi.yml
  type: http
slug: avoma-authentication
source_filename: avoma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: derived\nsource: openapi/avoma-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Avoma uses bearer token for authentication of the client. For now, you will have\n    to contact [Avoma Support](mailto:help@avoma.com) to get one issued for you.\n  sources:\n  - openapi/avoma-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/authentication/avoma-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Meeting-Assistant
- Sales-Enablement
- Automation
- Productivity
---
