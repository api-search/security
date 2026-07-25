---
api_key_in:
- header
api_specs:
- filename: salesforce-streaming-api-asyncapi.yml
  format: yaml
  label: Service Cloud Streaming API
  slug: service-cloud-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/asyncapi/salesforce-streaming-api-asyncapi.yml
- filename: salesforce-service-cloud-accounts-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Accounts API
  slug: salesforce-service-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-accounts-api-openapi.yml
- filename: salesforce-service-cloud-availability-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Availability API
  slug: salesforce-service-cloud-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-availability-api-openapi.yml
- filename: salesforce-service-cloud-cases-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Cases API
  slug: salesforce-service-cloud-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-cases-api-openapi.yml
- filename: salesforce-service-cloud-contacts-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Contacts API
  slug: salesforce-service-cloud-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-contacts-api-openapi.yml
- filename: salesforce-service-cloud-knowledge-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Knowledge API
  slug: salesforce-service-cloud-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-knowledge-api-openapi.yml
- filename: salesforce-service-cloud-messages-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Messages API
  slug: salesforce-service-cloud-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-messages-api-openapi.yml
- filename: salesforce-service-cloud-query-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Query API
  slug: salesforce-service-cloud-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-query-api-openapi.yml
- filename: salesforce-service-cloud-search-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Search API
  slug: salesforce-service-cloud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-search-api-openapi.yml
- filename: salesforce-service-cloud-sessions-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Sessions API
  slug: salesforce-service-cloud-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-sessions-api-openapi.yml
- filename: salesforce-service-cloud-settings-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Settings API
  slug: salesforce-service-cloud-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-settings-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Service Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salesforce Service Cloud secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salesforce Service Cloud
provider_slug: salesforce-service-cloud
scheme_count: 3
schemes:
- description: Live Agent API version header
  in: header
  name: apiKey
  parameter: X-LIVEAGENT-API-VERSION
  sources:
  - openapi/salesforce-live-agent-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-service-cloud-rest-openapi.yml
  type: oauth2
- bearerFormat: OAuth2
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-service-cloud-rest-openapi.yml
  type: http
slug: salesforce-service-cloud-authentication
source_filename: salesforce-service-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-live-agent-openapi.yml, openapi/salesforce-service-cloud-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-LIVEAGENT-API-VERSION\n  description: Live Agent API version header\n  sources:\n  - openapi/salesforce-live-agent-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/salesforce-service-cloud-rest-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  sources:\n  - openapi/salesforce-service-cloud-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/authentication/salesforce-service-cloud-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Case Management
- CRM
- Customer Service
- Help Desk
- Support
- Ticketing
---
