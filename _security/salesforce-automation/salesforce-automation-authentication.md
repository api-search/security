---
api_key_in: []
api_specs:
- filename: salesforce-rest-api-openapi.json
  format: json
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-rest-api-openapi.json
- filename: salesforce-bulk-api-openapi.json
  format: json
  label: Salesforce Bulk API 2.0
  slug: salesforce-bulk-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-bulk-api-openapi.json
- filename: salesforce-streaming-api-openapi.json
  format: json
  label: Salesforce Streaming API
  slug: salesforce-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-streaming-api-openapi.json
- filename: salesforce-platform-events-api-openapi.json
  format: json
  label: Salesforce Platform Events API
  slug: salesforce-platform-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-platform-events-api-openapi.json
- filename: salesforce-analytics-api-openapi.json
  format: json
  label: Salesforce Analytics API
  slug: salesforce-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-analytics-api-openapi.json
- filename: salesforce-tooling-api-openapi.json
  format: json
  label: Salesforce Tooling API
  slug: salesforce-tooling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-tooling-api-openapi.json
- filename: salesforce-connect-rest-api-openapi.json
  format: json
  label: Salesforce Connect REST API
  slug: salesforce-connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-connect-rest-api-openapi.json
- filename: salesforce-change-data-capture-api-openapi.json
  format: json
  label: Salesforce Change Data Capture API
  slug: salesforce-change-data-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-change-data-capture-api-openapi.json
- filename: salesforce-invocable-actions-api-openapi.json
  format: json
  label: Salesforce Invocable Actions API
  slug: salesforce-invocable-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-invocable-actions-api-openapi.json
- filename: salesforce-composite-api-openapi.json
  format: json
  label: Salesforce Composite API
  slug: salesforce-composite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-composite-api-openapi.json
- filename: salesforce-apex-rest-api-openapi.json
  format: json
  label: Salesforce Apex REST API
  slug: salesforce-apex-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/openapi/salesforce-apex-rest-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Automation Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salesforce Automation secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salesforce Automation
provider_slug: salesforce-automation
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-analytics-api-openapi.json
  - openapi/salesforce-apex-rest-api-openapi.json
  - openapi/salesforce-bulk-api-openapi.json
  - openapi/salesforce-change-data-capture-api-openapi.json
  - openapi/salesforce-composite-api-openapi.json
  - openapi/salesforce-connect-rest-api-openapi.json
  - openapi/salesforce-invocable-actions-api-openapi.json
  - openapi/salesforce-platform-events-api-openapi.json
  - openapi/salesforce-rest-api-openapi.json
  - openapi/salesforce-streaming-api-openapi.json
  - openapi/salesforce-tooling-api-openapi.json
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-analytics-api-openapi.json
  - openapi/salesforce-apex-rest-api-openapi.json
  - openapi/salesforce-bulk-api-openapi.json
  - openapi/salesforce-change-data-capture-api-openapi.json
  - openapi/salesforce-composite-api-openapi.json
  - openapi/salesforce-connect-rest-api-openapi.json
  - openapi/salesforce-invocable-actions-api-openapi.json
  - openapi/salesforce-platform-events-api-openapi.json
  - openapi/salesforce-rest-api-openapi.json
  - openapi/salesforce-streaming-api-openapi.json
  - openapi/salesforce-tooling-api-openapi.json
  type: http
slug: salesforce-automation-authentication
source_filename: salesforce-automation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-analytics-api-openapi.json, openapi/salesforce-apex-rest-api-openapi.json,\n  openapi/salesforce-bulk-api-openapi.json, openapi/salesforce-change-data-capture-api-openapi.json,\n  openapi/salesforce-composite-api-openapi.json, openapi/salesforce-connect-rest-api-openapi.json,\n  openapi/salesforce-invocable-actions-api-openapi.json, openapi/salesforce-platform-events-api-openapi.json,\n  openapi/salesforce-rest-api-openapi.json, openapi/salesforce-streaming-api-openapi.json, openapi/salesforce-tooling-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/salesforce-analytics-api-openapi.json\n  - openapi/salesforce-apex-rest-api-openapi.json\n\
  \  - openapi/salesforce-bulk-api-openapi.json\n  - openapi/salesforce-change-data-capture-api-openapi.json\n  - openapi/salesforce-composite-api-openapi.json\n  - openapi/salesforce-connect-rest-api-openapi.json\n  - openapi/salesforce-invocable-actions-api-openapi.json\n  - openapi/salesforce-platform-events-api-openapi.json\n  - openapi/salesforce-rest-api-openapi.json\n  - openapi/salesforce-streaming-api-openapi.json\n  - openapi/salesforce-tooling-api-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/salesforce-analytics-api-openapi.json\n  - openapi/salesforce-apex-rest-api-openapi.json\n  - openapi/salesforce-bulk-api-openapi.json\n  - openapi/salesforce-change-data-capture-api-openapi.json\n  - openapi/salesforce-composite-api-openapi.json\n  - openapi/salesforce-connect-rest-api-openapi.json\n  - openapi/salesforce-invocable-actions-api-openapi.json\n  - openapi/salesforce-platform-events-api-openapi.json\n  - openapi/salesforce-rest-api-openapi.json\n\
  \  - openapi/salesforce-streaming-api-openapi.json\n  - openapi/salesforce-tooling-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation/refs/heads/main/authentication/salesforce-automation-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Automation
- Cloud
- CRM
- Enterprise
- Sales
---
