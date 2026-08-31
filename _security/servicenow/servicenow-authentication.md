---
api_key_in: []
api_specs:
- filename: servicenow-events-asyncapi.yml
  format: yaml
  label: ServiceNow Event Management Topic Open API
  slug: servicenow-event-management-topic-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/asyncapi/servicenow-events-asyncapi.yml
- filename: servicenow-aggregate-statistics-api-openapi.yml
  format: yaml
  label: ServiceNow Aggregate Statistics API
  slug: servicenow-aggregate-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-aggregate-statistics-api-openapi.yml
- filename: servicenow-attachments-api-openapi.yml
  format: yaml
  label: ServiceNow Attachments API
  slug: servicenow-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-attachments-api-openapi.yml
- filename: servicenow-cart-api-openapi.yml
  format: yaml
  label: ServiceNow Cart API
  slug: servicenow-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-cart-api-openapi.yml
- filename: servicenow-catalog-items-api-openapi.yml
  format: yaml
  label: ServiceNow Catalog Items API
  slug: servicenow-catalog-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-catalog-items-api-openapi.yml
- filename: servicenow-catalogs-api-openapi.yml
  format: yaml
  label: ServiceNow Catalogs API
  slug: servicenow-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-catalogs-api-openapi.yml
- filename: servicenow-categories-api-openapi.yml
  format: yaml
  label: ServiceNow Categories API
  slug: servicenow-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-categories-api-openapi.yml
- filename: servicenow-change-tasks-api-openapi.yml
  format: yaml
  label: ServiceNow Change Tasks API
  slug: servicenow-change-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-change-tasks-api-openapi.yml
- filename: servicenow-cmdb-instances-api-openapi.yml
  format: yaml
  label: ServiceNow CMDB Instances API
  slug: servicenow-cmdb-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-cmdb-instances-api-openapi.yml
- filename: servicenow-contact-api-openapi.yml
  format: yaml
  label: ServiceNow Contact API
  slug: servicenow-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-contact-api-openapi.yml
- filename: servicenow-emergency-changes-api-openapi.yml
  format: yaml
  label: ServiceNow Emergency Changes API
  slug: servicenow-emergency-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-emergency-changes-api-openapi.yml
- filename: servicenow-import-sets-api-openapi.yml
  format: yaml
  label: ServiceNow Import Sets API
  slug: servicenow-import-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-import-sets-api-openapi.yml
- filename: servicenow-normal-changes-api-openapi.yml
  format: yaml
  label: ServiceNow Normal Changes API
  slug: servicenow-normal-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-normal-changes-api-openapi.yml
- filename: servicenow-standard-changes-api-openapi.yml
  format: yaml
  label: ServiceNow Standard Changes API
  slug: servicenow-standard-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-standard-changes-api-openapi.yml
- filename: servicenow-table-records-api-openapi.yml
  format: yaml
  label: ServiceNow Table Records API
  slug: servicenow-table-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-table-records-api-openapi.yml
- filename: servicenow-trouble-ticket-api-openapi.yml
  format: yaml
  label: ServiceNow Trouble Ticket API
  slug: servicenow-trouble-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-trouble-ticket-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Servicenow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: ServiceNow secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: ServiceNow
provider_slug: servicenow
scheme_count: 3
schemes:
- description: Basic authentication with ServiceNow credentials. User must have the csm_ws_integration role.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/contact-api-openapi.yaml
  - openapi/servicenow-aggregate-api-openapi.yml
  - openapi/servicenow-attachment-api-openapi.yml
  - openapi/servicenow-change-management-api-openapi.yml
  - openapi/servicenow-cmdb-instance-api-openapi.yml
  - openapi/servicenow-import-set-api-openapi.yml
  - openapi/servicenow-service-catalog-api-openapi.yml
  - openapi/servicenow-table-api-openapi.yml
  - openapi/trouble-ticket-openapi.yaml
  type: http
- description: OAuth 2.0 authentication using ServiceNow's OAuth provider.
  flows:
  - flow: password
    scopes: 0
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  name: oauth2
  sources:
  - openapi/servicenow-aggregate-api-openapi.yml
  - openapi/servicenow-attachment-api-openapi.yml
  - openapi/servicenow-change-management-api-openapi.yml
  - openapi/servicenow-cmdb-instance-api-openapi.yml
  - openapi/servicenow-import-set-api-openapi.yml
  - openapi/servicenow-service-catalog-api-openapi.yml
  type: oauth2
- description: OAuth 2.0 authentication using ServiceNow's OAuth provider. Requires a registered OAuth application on the instance.
  flows:
  - authorizationUrl: https://{instance}.service-now.com/oauth_auth.do
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  - flow: password
    scopes: 0
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  name: oauth2
  sources:
  - openapi/servicenow-table-api-openapi.yml
  type: oauth2
slug: servicenow-authentication
source_filename: servicenow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contact-api-openapi.yaml, openapi/servicenow-aggregate-api-openapi.yml, openapi/servicenow-attachment-api-openapi.yml,\n  openapi/servicenow-change-management-api-openapi.yml, openapi/servicenow-cmdb-instance-api-openapi.yml,\n  openapi/servicenow-import-set-api-openapi.yml, openapi/servicenow-service-catalog-api-openapi.yml,\n  openapi/servicenow-table-api-openapi.yml, openapi/trouble-ticket-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - password\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication with ServiceNow credentials. User must have the csm_ws_integration\n    role.\n  sources:\n  - openapi/contact-api-openapi.yaml\n  - openapi/servicenow-aggregate-api-openapi.yml\n  - openapi/servicenow-attachment-api-openapi.yml\n  - openapi/servicenow-change-management-api-openapi.yml\n  - openapi/servicenow-cmdb-instance-api-openapi.yml\n\
  \  - openapi/servicenow-import-set-api-openapi.yml\n  - openapi/servicenow-service-catalog-api-openapi.yml\n  - openapi/servicenow-table-api-openapi.yml\n  - openapi/trouble-ticket-openapi.yaml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n    scopes: 0\n  description: OAuth 2.0 authentication using ServiceNow's OAuth provider.\n  sources:\n  - openapi/servicenow-aggregate-api-openapi.yml\n  - openapi/servicenow-attachment-api-openapi.yml\n  - openapi/servicenow-change-management-api-openapi.yml\n  - openapi/servicenow-cmdb-instance-api-openapi.yml\n  - openapi/servicenow-import-set-api-openapi.yml\n  - openapi/servicenow-service-catalog-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{instance}.service-now.com/oauth_auth.do\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n    scopes: 0\n  - flow: password\n    tokenUrl:\
  \ https://{instance}.service-now.com/oauth_token.do\n    scopes: 0\n  description: OAuth 2.0 authentication using ServiceNow's OAuth provider. Requires a registered\n    OAuth application on the instance.\n  sources:\n  - openapi/servicenow-table-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/authentication/servicenow-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow-Automation
- Workflows
---
