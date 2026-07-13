---
api_key_in:
- header
api_specs:
- filename: amplitude-http-v2-api-openapi.yml
  format: yaml
  label: Amplitude HTTP V2 API
  slug: http-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-http-v2-api-openapi.yml
- filename: amplitude-identify-api-openapi.yml
  format: yaml
  label: Amplitude Identify API
  slug: identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-identify-api-openapi.yml
- filename: amplitude-dashboard-rest-api-openapi.yml
  format: yaml
  label: Amplitude Dashboard REST API
  slug: dashboard-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-dashboard-rest-api-openapi.yml
- filename: amplitude-export-api-openapi.yml
  format: yaml
  label: Amplitude Export API
  slug: export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-export-api-openapi.yml
- filename: amplitude-behavioral-cohorts-api-openapi.yml
  format: yaml
  label: Amplitude Behavioral Cohorts API
  slug: behavioral-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-behavioral-cohorts-api-openapi.yml
- filename: amplitude-taxonomy-api-openapi.yml
  format: yaml
  label: Amplitude Taxonomy API
  slug: taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-taxonomy-api-openapi.yml
- filename: amplitude-attribution-api-openapi.yml
  format: yaml
  label: Amplitude Attribution API
  slug: attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-attribution-api-openapi.yml
- filename: amplitude-chart-annotations-api-openapi.yml
  format: yaml
  label: Amplitude Chart Annotations API
  slug: chart-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-chart-annotations-api-openapi.yml
- filename: amplitude-user-profile-api-openapi.yml
  format: yaml
  label: Amplitude User Profile API
  slug: user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-user-profile-api-openapi.yml
- filename: amplitude-user-mapping-api-openapi.yml
  format: yaml
  label: Amplitude User Mapping API
  slug: user-mapping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-user-mapping-api-openapi.yml
- filename: amplitude-scim-api-openapi.yml
  format: yaml
  label: Amplitude SCIM API
  slug: scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-scim-api-openapi.yml
- filename: amplitude-dsar-api-openapi.yml
  format: yaml
  label: Amplitude Data Subject Access Request API
  slug: dsar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-dsar-api-openapi.yml
- filename: amplitude-experiment-evaluation-api-openapi.yml
  format: yaml
  label: Amplitude Experiment Evaluation API
  slug: experiment-evaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-experiment-evaluation-api-openapi.yml
- filename: amplitude-experiment-management-api-openapi.yml
  format: yaml
  label: Amplitude Experiment Management API
  slug: experiment-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/openapi/amplitude-experiment-management-api-openapi.yml
- filename: amplitude-webhooks-cohort-sync-asyncapi.yml
  format: yaml
  label: Amplitude Webhooks and Cohort Sync
  slug: webhooks-cohort-sync
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/asyncapi/amplitude-webhooks-cohort-sync-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amplitude Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amplitude secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Amplitude
provider_slug: amplitude
scheme_count: 3
schemes:
- description: Use your Amplitude API key as the username and your secret key as the password. Encode them as base64 in the format api_key:secret_key.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/amplitude-behavioral-cohorts-api-openapi.yml
  - openapi/amplitude-chart-annotations-api-openapi.yml
  - openapi/amplitude-dashboard-rest-api-openapi.yml
  - openapi/amplitude-dsar-api-openapi.yml
  - openapi/amplitude-export-api-openapi.yml
  - openapi/amplitude-taxonomy-api-openapi.yml
  - openapi/amplitude-user-mapping-api-openapi.yml
  type: http
- description: Pass your deployment key in the Authorization header with the prefix Api-Key, for example Api-Key YOUR_DEPLOYMENT_KEY.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/amplitude-experiment-evaluation-api-openapi.yml
  - openapi/amplitude-user-profile-api-openapi.yml
  type: apiKey
- description: Use a Management API key generated in the Experiment sidebar of the Amplitude UI. Pass it in the Authorization header as Bearer YOUR_MANAGEMENT_API_KEY.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/amplitude-experiment-management-api-openapi.yml
  - openapi/amplitude-scim-api-openapi.yml
  type: http
slug: amplitude-authentication
source_filename: amplitude-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amplitude-behavioral-cohorts-api-openapi.yml, openapi/amplitude-chart-annotations-api-openapi.yml,\n  openapi/amplitude-dashboard-rest-api-openapi.yml, openapi/amplitude-dsar-api-openapi.yml,\n  openapi/amplitude-experiment-evaluation-api-openapi.yml, openapi/amplitude-experiment-management-api-openapi.yml,\n  openapi/amplitude-export-api-openapi.yml, openapi/amplitude-scim-api-openapi.yml, openapi/amplitude-taxonomy-api-openapi.yml,\n  openapi/amplitude-user-mapping-api-openapi.yml, openapi/amplitude-user-profile-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your Amplitude API key as the username and your secret key as the password.\n    Encode them as base64 in the format api_key:secret_key.\n  sources:\n  - openapi/amplitude-behavioral-cohorts-api-openapi.yml\n  - openapi/amplitude-chart-annotations-api-openapi.yml\n\
  \  - openapi/amplitude-dashboard-rest-api-openapi.yml\n  - openapi/amplitude-dsar-api-openapi.yml\n  - openapi/amplitude-export-api-openapi.yml\n  - openapi/amplitude-taxonomy-api-openapi.yml\n  - openapi/amplitude-user-mapping-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Pass your deployment key in the Authorization header with the prefix Api-Key,\n    for example Api-Key YOUR_DEPLOYMENT_KEY.\n  sources:\n  - openapi/amplitude-experiment-evaluation-api-openapi.yml\n  - openapi/amplitude-user-profile-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Use a Management API key generated in the Experiment sidebar of the Amplitude\n    UI. Pass it in the Authorization header as Bearer YOUR_MANAGEMENT_API_KEY.\n  sources:\n  - openapi/amplitude-experiment-management-api-openapi.yml\n  - openapi/amplitude-scim-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/authentication/amplitude-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
---
