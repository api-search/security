---
api_key_in: []
api_specs:
- filename: swagger-v3.v3.json
  format: json
  label: Jira Cloud Platform REST API
  slug: jira-cloud-platform-rest-api
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/jira/platform/swagger-v3.v3.json
- filename: swagger.v3.json
  format: json
  label: Jira Software Cloud REST API
  slug: jira-software-cloud-rest-api
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- filename: swagger.v3.json
  format: json
  label: Jira Service Management REST API
  slug: jira-service-management-rest-api
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Atlassian Jira Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Atlassian Jira secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Atlassian Jira
provider_slug: atlassian-jira
scheme_count: 2
schemes:
- description: Email + API token via HTTP Basic auth.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/atlassian-jira-openapi.yml
  type: http
- description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: OAuth2
  sources:
  - openapi/atlassian-jira-openapi.yml
  type: oauth2
slug: atlassian-jira-authentication
source_filename: atlassian-jira-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atlassian-jira-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Email + API token via HTTP Basic auth.\n  sources:\n  - openapi/atlassian-jira-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n    scopes: 4\n  description: Atlassian OAuth 2.0 (3LO) for Jira Cloud.\n  sources:\n  - openapi/atlassian-jira-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/authentication/atlassian-jira-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Agile
- Atlassian
- Bug Tracking
- Issue Tracking
- ITSM
- Kanban
- Project Management
- Scrum
- Service Desk
---
