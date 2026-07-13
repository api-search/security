---
api_key_in:
- header
api_specs:
- filename: resources_list.htm
  format: yaml
  label: Salesforce Service Cloud REST API
  slug: salesforce-service-cloud-rest-api
  spec_type: OpenAPI
  url: https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/resources_list.htm
- filename: salesforce-streaming-api-asyncapi.yml
  format: yaml
  label: Service Cloud Streaming API
  slug: service-cloud-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/asyncapi/salesforce-streaming-api-asyncapi.yml
- filename: salesforce-live-agent-openapi.yml
  format: yaml
  label: Live Agent REST API
  slug: live-agent-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-live-agent-openapi.yml
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
