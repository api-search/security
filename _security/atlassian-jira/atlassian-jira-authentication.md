---
api_key_in: []
api_specs:
- filename: atlassian-jira-fields-api-openapi.yml
  format: yaml
  label: Atlassian Jira Fields API
  slug: atlassian-jira-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-fields-api-openapi.yml
- filename: atlassian-jira-issue-comments-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issue Comments API
  slug: atlassian-jira-issue-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issue-comments-api-openapi.yml
- filename: atlassian-jira-issue-search-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issue Search API
  slug: atlassian-jira-issue-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issue-search-api-openapi.yml
- filename: atlassian-jira-issue-transitions-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issue Transitions API
  slug: atlassian-jira-issue-transitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issue-transitions-api-openapi.yml
- filename: atlassian-jira-issue-worklogs-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issue Worklogs API
  slug: atlassian-jira-issue-worklogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issue-worklogs-api-openapi.yml
- filename: atlassian-jira-issues-api-openapi.yml
  format: yaml
  label: Atlassian Jira Issues API
  slug: atlassian-jira-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-issues-api-openapi.yml
- filename: atlassian-jira-projects-api-openapi.yml
  format: yaml
  label: Atlassian Jira Projects API
  slug: atlassian-jira-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-projects-api-openapi.yml
- filename: atlassian-jira-users-api-openapi.yml
  format: yaml
  label: Atlassian Jira Users API
  slug: atlassian-jira-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/openapi/atlassian-jira-users-api-openapi.yml
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
