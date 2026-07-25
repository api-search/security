---
api_key_in: []
api_specs:
- filename: jira-issue-comments-api-openapi.yml
  format: yaml
  label: Jira Issue Comments API
  slug: jira-issue-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-comments-api-openapi.yml
- filename: jira-issue-priorities-api-openapi.yml
  format: yaml
  label: Jira Issue Priorities API
  slug: jira-issue-priorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-priorities-api-openapi.yml
- filename: jira-issue-search-api-openapi.yml
  format: yaml
  label: Jira Issue Search API
  slug: jira-issue-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-search-api-openapi.yml
- filename: jira-issue-statuses-api-openapi.yml
  format: yaml
  label: Jira Issue Statuses API
  slug: jira-issue-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-statuses-api-openapi.yml
- filename: jira-issue-transitions-api-openapi.yml
  format: yaml
  label: Jira Issue Transitions API
  slug: jira-issue-transitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-transitions-api-openapi.yml
- filename: jira-issue-types-api-openapi.yml
  format: yaml
  label: Jira Issue Types API
  slug: jira-issue-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-types-api-openapi.yml
- filename: jira-issues-api-openapi.yml
  format: yaml
  label: Jira Issues API
  slug: jira-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issues-api-openapi.yml
- filename: jira-projects-api-openapi.yml
  format: yaml
  label: Jira Projects API
  slug: jira-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-projects-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Jira Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Jira secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Jira
provider_slug: jira
scheme_count: 3
schemes:
- description: 'Basic authentication using an Atlassian account email and API token. Format: email:api_token, Base64 encoded. Generate API tokens at https://id.atlassian.com/manage-profile/security/api-tokens.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/jira-cloud-platform-rest-api-openapi.yml
  type: http
- description: OAuth 2.0 authorization code grant (3LO) for Jira Cloud apps.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oauth2
  sources:
  - openapi/jira-cloud-platform-rest-api-openapi.yml
  type: oauth2
- description: Bearer token authentication using a personal access token (PAT) or OAuth 2.0 access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jira-cloud-platform-rest-api-openapi.yml
  type: http
slug: jira-authentication
source_filename: jira-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jira-cloud-platform-rest-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Basic authentication using an Atlassian account email and API token. Format:\n    email:api_token, Base64 encoded. Generate API tokens at https://id.atlassian.com/manage-profile/security/api-tokens.'\n  sources:\n  - openapi/jira-cloud-platform-rest-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n    scopes: 5\n  description: OAuth 2.0 authorization code grant (3LO) for Jira Cloud apps.\n  sources:\n  - openapi/jira-cloud-platform-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using a personal access\
  \ token (PAT) or OAuth 2.0\n    access token.\n  sources:\n  - openapi/jira-cloud-platform-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/authentication/jira-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
---
