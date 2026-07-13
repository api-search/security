---
api_key_in: []
api_specs:
- filename: salesforce-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-openapi.yml
- filename: salesforce-bulk-api-2-openapi.yml
  format: yaml
  label: Salesforce Bulk API 2.0
  slug: salesforce-bulk-api-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-bulk-api-2-openapi.yml
- filename: salesforce-streaming-asyncapi.yml
  format: yaml
  label: Salesforce Streaming API
  slug: salesforce-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/asyncapi/salesforce-streaming-asyncapi.yml
- filename: salesforce-platform-events-asyncapi.yml
  format: yaml
  label: Salesforce Platform Events API
  slug: salesforce-platform-events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/asyncapi/salesforce-platform-events-asyncapi.yml
- filename: salesforce-change-data-capture-asyncapi.yml
  format: yaml
  label: Salesforce Change Data Capture API
  slug: salesforce-change-data-capture-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/asyncapi/salesforce-change-data-capture-asyncapi.yml
- filename: salesforce-ui-api-openapi.yml
  format: yaml
  label: Salesforce UI API
  slug: salesforce-ui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-ui-api-openapi.yml
- filename: salesforce-marketing-cloud-rest-openapi.yml
  format: yaml
  label: Salesforce Marketing Cloud REST API
  slug: salesforce-marketing-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-marketing-cloud-rest-openapi.yml
- filename: salesforce-openapi.yml
  format: yaml
  label: Salesforce
  slug: salesforce-salesforce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/openapi/salesforce-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Salesforce secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Salesforce
provider_slug: salesforce
scheme_count: 2
schemes:
- description: OAuth 2.0 Bearer token obtained from the Salesforce OAuth 2.0 token endpoint. Include this token in the Authorization header as "Bearer {access_token}".
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-bulk-api-2-openapi.yml
  - openapi/salesforce-marketing-cloud-rest-openapi.yml
  - openapi/salesforce-rest-api-openapi.yml
  - openapi/salesforce-ui-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: '{DefaultParameterValue}{DefaultParameterValue}/services/oauth2/authorize'
    flow: implicit
    scopes: 1
  name: oauth2
  sources:
  - openapi/salesforce-openapi.yml
  type: oauth2
slug: salesforce-authentication
source_filename: salesforce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-bulk-api-2-openapi.yml, openapi/salesforce-marketing-cloud-rest-openapi.yml,\n  openapi/salesforce-openapi.yml, openapi/salesforce-rest-api-openapi.yml, openapi/salesforce-ui-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token obtained from the Salesforce OAuth 2.0 token endpoint.\n    Include this token in the Authorization header as \"Bearer {access_token}\".\n  sources:\n  - openapi/salesforce-bulk-api-2-openapi.yml\n  - openapi/salesforce-marketing-cloud-rest-openapi.yml\n  - openapi/salesforce-rest-api-openapi.yml\n  - openapi/salesforce-ui-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: '{DefaultParameterValue}{DefaultParameterValue}/services/oauth2/authorize'\n    scopes: 1\n  sources:\n  - openapi/salesforce-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/authentication/salesforce-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fortune 500
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
---
