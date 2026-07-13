---
api_key_in:
- query
api_specs:
- filename: openapi
  format: yaml
  label: Mixpanel Ingestion API
  slug: mixpanel-ingestion-api
  spec_type: OpenAPI
  url: https://developer.mixpanel.com/reference/openapi
- filename: openapi
  format: yaml
  label: Mixpanel Query API
  slug: mixpanel-query-api
  spec_type: OpenAPI
  url: https://developer.mixpanel.com/reference/openapi
- filename: openapi
  format: yaml
  label: Mixpanel Data Pipelines API
  slug: mixpanel-data-pipelines-api
  spec_type: OpenAPI
  url: https://developer.mixpanel.com/reference/openapi
- filename: mixpanel-identity-openapi.yml
  format: yaml
  label: Mixpanel Identity API
  slug: mixpanel-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-identity-openapi.yml
- filename: mixpanel-event-export-openapi.yml
  format: yaml
  label: Mixpanel Event Export API
  slug: mixpanel-event-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-event-export-openapi.yml
- filename: mixpanel-lexicon-schemas-openapi.yml
  format: yaml
  label: Mixpanel Lexicon Schemas API
  slug: mixpanel-lexicon-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-lexicon-schemas-openapi.yml
- filename: mixpanel-service-accounts-openapi.yml
  format: yaml
  label: Mixpanel Service Accounts API
  slug: mixpanel-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-service-accounts-openapi.yml
- filename: mixpanel-annotations-openapi.yml
  format: yaml
  label: Mixpanel Annotations API
  slug: mixpanel-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-annotations-openapi.yml
- filename: mixpanel-gdpr-ccpa-openapi.yml
  format: yaml
  label: Mixpanel GDPR and CCPA API
  slug: mixpanel-gdpr-and-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-gdpr-ccpa-openapi.yml
- filename: mixpanel-warehouse-connectors-openapi.yml
  format: yaml
  label: Mixpanel Warehouse Connectors API
  slug: mixpanel-warehouse-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-warehouse-connectors-openapi.yml
- filename: mixpanel-webhooks-asyncapi.yml
  format: yaml
  label: Mixpanel Webhooks
  slug: mixpanel-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/asyncapi/mixpanel-webhooks-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mixpanel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mixpanel secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mixpanel
provider_slug: mixpanel
scheme_count: 3
schemes:
- description: Service account credentials for API authentication.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mixpanel-annotations-openapi.yml
  - openapi/mixpanel-data-pipelines-openapi.yml
  - openapi/mixpanel-event-export-openapi.yml
  - openapi/mixpanel-identity-openapi.yml
  - openapi/mixpanel-ingestion-openapi.yml
  - openapi/mixpanel-lexicon-schemas-openapi.yml
  - openapi/mixpanel-query-openapi.yml
  - openapi/mixpanel-service-accounts-openapi.yml
  - openapi/mixpanel-warehouse-connectors-openapi.yml
  type: http
- description: OAuth 2.0 bearer token for GDPR API authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mixpanel-gdpr-ccpa-openapi.yml
  type: http
- description: Mixpanel project token for client-side tracking
  in: query
  name: projectToken
  parameter: token
  sources:
  - openapi/mixpanel-ingestion-openapi.yml
  type: apiKey
slug: mixpanel-authentication
source_filename: mixpanel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mixpanel-annotations-openapi.yml, openapi/mixpanel-data-pipelines-openapi.yml,\n  openapi/mixpanel-event-export-openapi.yml, openapi/mixpanel-gdpr-ccpa-openapi.yml, openapi/mixpanel-identity-openapi.yml,\n  openapi/mixpanel-ingestion-openapi.yml, openapi/mixpanel-lexicon-schemas-openapi.yml, openapi/mixpanel-query-openapi.yml,\n  openapi/mixpanel-service-accounts-openapi.yml, openapi/mixpanel-warehouse-connectors-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Service account credentials for API authentication.\n  sources:\n  - openapi/mixpanel-annotations-openapi.yml\n  - openapi/mixpanel-data-pipelines-openapi.yml\n  - openapi/mixpanel-event-export-openapi.yml\n  - openapi/mixpanel-identity-openapi.yml\n  - openapi/mixpanel-ingestion-openapi.yml\n  - openapi/mixpanel-lexicon-schemas-openapi.yml\n  - openapi/mixpanel-query-openapi.yml\n\
  \  - openapi/mixpanel-service-accounts-openapi.yml\n  - openapi/mixpanel-warehouse-connectors-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token for GDPR API authentication.\n  sources:\n  - openapi/mixpanel-gdpr-ccpa-openapi.yml\n- name: projectToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Mixpanel project token for client-side tracking\n  sources:\n  - openapi/mixpanel-ingestion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/authentication/mixpanel-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Analytics
- Data Analysis
- Event Tracking
- Product Analytics
- User Behavior
---
