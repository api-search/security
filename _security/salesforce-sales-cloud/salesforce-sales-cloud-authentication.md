---
api_key_in: []
api_specs:
- filename: salesforce-sales-cloud-rest-api-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-rest-api-openapi.yml
- filename: salesforce-sales-cloud-bulk-api-openapi.yml
  format: yaml
  label: Bulk API 2.0
  slug: bulk-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-bulk-api-openapi.yml
- filename: salesforce-sales-cloud-platform-events-api-openapi.yml
  format: yaml
  label: Platform Events API
  slug: platform-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-platform-events-api-openapi.yml
- filename: salesforce-sales-cloud-analytics-api-openapi.yml
  format: yaml
  label: Analytics REST API
  slug: analytics-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-analytics-api-openapi.yml
- filename: salesforce-sales-cloud-composite-api-openapi.yml
  format: yaml
  label: Salesforce Composite API
  slug: salesforce-composite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-composite-api-openapi.yml
- filename: salesforce-sales-cloud-graphql-api-openapi.yml
  format: yaml
  label: Salesforce GraphQL API
  slug: salesforce-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-graphql-api-openapi.yml
- filename: salesforce-sales-cloud-tooling-api-openapi.yml
  format: yaml
  label: Salesforce Tooling API
  slug: salesforce-tooling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-tooling-api-openapi.yml
- filename: salesforce-sales-cloud-change-data-capture-api-openapi.yml
  format: yaml
  label: Salesforce Change Data Capture API
  slug: salesforce-change-data-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml
- filename: salesforce-sales-cloud-connect-api-openapi.yml
  format: yaml
  label: Salesforce Connect REST API
  slug: salesforce-connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-connect-api-openapi.yml
- filename: salesforce-sales-cloud-ui-api-openapi.yml
  format: yaml
  label: Salesforce User Interface API
  slug: salesforce-user-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-ui-api-openapi.yml
- filename: salesforce-sales-cloud-apex-rest-api-openapi.yml
  format: yaml
  label: Salesforce Apex REST API
  slug: salesforce-apex-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Sales Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Salesforce Sales Cloud secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Salesforce Sales Cloud
provider_slug: salesforce-sales-cloud
scheme_count: 3
schemes:
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-sales-cloud-analytics-api-openapi.yml
  - openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml
  - openapi/salesforce-sales-cloud-bulk-api-openapi.yml
  - openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml
  - openapi/salesforce-sales-cloud-composite-api-openapi.yml
  - openapi/salesforce-sales-cloud-connect-api-openapi.yml
  - openapi/salesforce-sales-cloud-graphql-api-openapi.yml
  - openapi/salesforce-sales-cloud-platform-events-api-openapi.yml
  - openapi/salesforce-sales-cloud-tooling-api-openapi.yml
  - openapi/salesforce-sales-cloud-ui-api-openapi.yml
  type: oauth2
- bearerFormat: OAuth 2.0 Access Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-sales-cloud-analytics-api-openapi.yml
  - openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml
  - openapi/salesforce-sales-cloud-bulk-api-openapi.yml
  - openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml
  - openapi/salesforce-sales-cloud-composite-api-openapi.yml
  - openapi/salesforce-sales-cloud-connect-api-openapi.yml
  - openapi/salesforce-sales-cloud-graphql-api-openapi.yml
  - openapi/salesforce-sales-cloud-platform-events-api-openapi.yml
  - openapi/salesforce-sales-cloud-rest-api-openapi.yml
  - openapi/salesforce-sales-cloud-tooling-api-openapi.yml
  - openapi/salesforce-sales-cloud-ui-api-openapi.yml
  type: http
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-sales-cloud-rest-api-openapi.yml
  type: oauth2
slug: salesforce-sales-cloud-authentication
source_filename: salesforce-sales-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-sales-cloud-analytics-api-openapi.yml, openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml,\n  openapi/salesforce-sales-cloud-bulk-api-openapi.yml, openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml,\n  openapi/salesforce-sales-cloud-composite-api-openapi.yml, openapi/salesforce-sales-cloud-connect-api-openapi.yml,\n  openapi/salesforce-sales-cloud-graphql-api-openapi.yml, openapi/salesforce-sales-cloud-platform-events-api-openapi.yml,\n  openapi/salesforce-sales-cloud-rest-api-openapi.yml, openapi/salesforce-sales-cloud-tooling-api-openapi.yml,\n  openapi/salesforce-sales-cloud-ui-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n\
  \    scopes: 1\n  description: Salesforce OAuth 2.0 authentication\n  sources:\n  - openapi/salesforce-sales-cloud-analytics-api-openapi.yml\n  - openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml\n  - openapi/salesforce-sales-cloud-bulk-api-openapi.yml\n  - openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml\n  - openapi/salesforce-sales-cloud-composite-api-openapi.yml\n  - openapi/salesforce-sales-cloud-connect-api-openapi.yml\n  - openapi/salesforce-sales-cloud-graphql-api-openapi.yml\n  - openapi/salesforce-sales-cloud-platform-events-api-openapi.yml\n  - openapi/salesforce-sales-cloud-tooling-api-openapi.yml\n  - openapi/salesforce-sales-cloud-ui-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth 2.0 Access Token\n  sources:\n  - openapi/salesforce-sales-cloud-analytics-api-openapi.yml\n  - openapi/salesforce-sales-cloud-apex-rest-api-openapi.yml\n  - openapi/salesforce-sales-cloud-bulk-api-openapi.yml\n  - openapi/salesforce-sales-cloud-change-data-capture-api-openapi.yml\n\
  \  - openapi/salesforce-sales-cloud-composite-api-openapi.yml\n  - openapi/salesforce-sales-cloud-connect-api-openapi.yml\n  - openapi/salesforce-sales-cloud-graphql-api-openapi.yml\n  - openapi/salesforce-sales-cloud-platform-events-api-openapi.yml\n  - openapi/salesforce-sales-cloud-rest-api-openapi.yml\n  - openapi/salesforce-sales-cloud-tooling-api-openapi.yml\n  - openapi/salesforce-sales-cloud-ui-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 3\n  - flow: clientCredentials\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 1\n  description: Salesforce OAuth 2.0 authentication\n  sources:\n  - openapi/salesforce-sales-cloud-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/authentication/salesforce-sales-cloud-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
---
