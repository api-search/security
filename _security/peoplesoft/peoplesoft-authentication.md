---
api_key_in: []
api_specs:
- filename: rest-api.yml
  format: yaml
  label: PeopleSoft REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/rest-api.yml
- filename: application-services-framework.yml
  format: yaml
  label: PeopleSoft Application Services Framework API
  slug: application-services-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/application-services-framework.yml
- filename: integration-broker.yml
  format: yaml
  label: PeopleSoft Integration Broker
  slug: integration-broker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/integration-broker.yml
- filename: query.yml
  format: yaml
  label: PeopleSoft Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/query.yml
- filename: component-interface.yml
  format: yaml
  label: PeopleSoft Component Interface API
  slug: component-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/component-interface.yml
- filename: search-framework.yml
  format: yaml
  label: PeopleSoft Search Framework API
  slug: search-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/search-framework.yml
- filename: notification-framework.yml
  format: yaml
  label: PeopleSoft Notification Framework API
  slug: notification-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/notification-framework.yml
- filename: chatbot-integration.yml
  format: yaml
  label: PeopleSoft Chatbot Integration Framework API
  slug: chatbot-integration-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/chatbot-integration.yml
- filename: approval-workflow-engine.yml
  format: yaml
  label: PeopleSoft Approval Workflow Engine API
  slug: approval-workflow-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/approval-workflow-engine.yml
- filename: process-scheduler.yml
  format: yaml
  label: PeopleSoft Process Scheduler API
  slug: process-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/process-scheduler.yml
- filename: cloud-manager.yml
  format: yaml
  label: PeopleSoft Cloud Manager API
  slug: cloud-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/cloud-manager.yml
- filename: update-manager.yml
  format: yaml
  label: PeopleSoft Update Manager API
  slug: update-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/update-manager.yml
- filename: pivot-grid.yml
  format: yaml
  label: PeopleSoft Pivot Grid API
  slug: pivot-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/pivot-grid.yml
- filename: hcm.yml
  format: yaml
  label: PeopleSoft HCM API
  slug: hcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/hcm.yml
- filename: recruiting-talent-management.yml
  format: yaml
  label: PeopleSoft Recruiting and Talent Management API
  slug: recruiting-and-talent-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/recruiting-talent-management.yml
- filename: financials.yml
  format: yaml
  label: PeopleSoft Financials API
  slug: financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/financials.yml
- filename: supply-chain-management.yml
  format: yaml
  label: PeopleSoft Supply Chain Management API
  slug: supply-chain-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/supply-chain-management.yml
- filename: crm.yml
  format: yaml
  label: PeopleSoft CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/crm.yml
- filename: campus-solutions.yml
  format: yaml
  label: PeopleSoft Campus Solutions API
  slug: campus-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/campus-solutions.yml
- filename: enterprise-performance-management.yml
  format: yaml
  label: PeopleSoft Enterprise Performance Management API
  slug: enterprise-performance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/enterprise-performance-management.yml
- filename: interaction-hub.yml
  format: yaml
  label: PeopleSoft Interaction Hub API
  slug: interaction-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/interaction-hub.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Peoplesoft Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: PeopleSoft secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: PeopleSoft
provider_slug: peoplesoft
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/application-services-framework.yml
  - openapi/approval-workflow-engine.yml
  - openapi/campus-solutions.yml
  - openapi/chatbot-integration.yml
  - openapi/cloud-manager.yml
  - openapi/component-interface.yml
  - openapi/crm.yml
  - openapi/enterprise-performance-management.yml
  - openapi/financials.yml
  - openapi/hcm.yml
  - openapi/integration-broker.yml
  - openapi/interaction-hub.yml
  - openapi/notification-framework.yml
  - openapi/pivot-grid.yml
  - openapi/process-scheduler.yml
  - openapi/query.yml
  - openapi/recruiting-talent-management.yml
  - openapi/rest-api.yml
  - openapi/search-framework.yml
  - openapi/supply-chain-management.yml
  - openapi/update-manager.yml
  type: http
- flows:
  - authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{hostname}:{port}/psft/oauth/token
  name: oauth2
  sources:
  - openapi/application-services-framework.yml
  - openapi/rest-api.yml
  type: oauth2
slug: peoplesoft-authentication
source_filename: peoplesoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/application-services-framework.yml, openapi/approval-workflow-engine.yml, openapi/campus-solutions.yml,\n  openapi/chatbot-integration.yml, openapi/cloud-manager.yml, openapi/component-interface.yml,\n  openapi/crm.yml, openapi/enterprise-performance-management.yml, openapi/financials.yml, openapi/hcm.yml,\n  openapi/integration-broker.yml, openapi/interaction-hub.yml ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/application-services-framework.yml\n  - openapi/approval-workflow-engine.yml\n  - openapi/campus-solutions.yml\n  - openapi/chatbot-integration.yml\n  - openapi/cloud-manager.yml\n  - openapi/component-interface.yml\n  - openapi/crm.yml\n  - openapi/enterprise-performance-management.yml\n  - openapi/financials.yml\n  - openapi/hcm.yml\n  - openapi/integration-broker.yml\n  - openapi/interaction-hub.yml\n\
  \  - openapi/notification-framework.yml\n  - openapi/pivot-grid.yml\n  - openapi/process-scheduler.yml\n  - openapi/query.yml\n  - openapi/recruiting-talent-management.yml\n  - openapi/rest-api.yml\n  - openapi/search-framework.yml\n  - openapi/supply-chain-management.yml\n  - openapi/update-manager.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize\n    tokenUrl: https://{hostname}:{port}/psft/oauth/token\n    scopes: 0\n  sources:\n  - openapi/application-services-framework.yml\n  - openapi/rest-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/authentication/peoplesoft-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
---
