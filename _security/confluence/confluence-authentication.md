---
api_key_in: []
api_specs:
- filename: confluence-space-api-openapi.yml
  format: yaml
  label: Confluence Space API
  slug: confluence-space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/openapi/confluence-space-api-openapi.yml
- filename: confluence-attachment-api-openapi.yml
  format: yaml
  label: Confluence Attachment API
  slug: confluence-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/openapi/confluence-attachment-api-openapi.yml
- filename: confluence-blog-post-api-openapi.yml
  format: yaml
  label: Confluence Blog Post API
  slug: confluence-blog-post-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/openapi/confluence-blog-post-api-openapi.yml
- filename: confluence-comment-api-openapi.yml
  format: yaml
  label: Confluence Comment API
  slug: confluence-comment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/openapi/confluence-comment-api-openapi.yml
- filename: confluence-label-api-openapi.yml
  format: yaml
  label: Confluence Label API
  slug: confluence-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/openapi/confluence-label-api-openapi.yml
- filename: confluence-page-api-openapi.yml
  format: yaml
  label: Confluence Page API
  slug: confluence-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/openapi/confluence-page-api-openapi.yml
- filename: confluence-space-api-openapi.yml
  format: yaml
  label: Confluence Space API
  slug: confluence-space-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/openapi/confluence-space-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Confluence Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Confluence secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Confluence
provider_slug: confluence
scheme_count: 3
schemes:
- description: Basic authentication using email and API token. Provide your Atlassian account email as the username and an API token as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/confluence-cloud-v2.yml
  type: http
- description: OAuth 2.0 (3LO) for Confluence Cloud apps.
  flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://auth.atlassian.com/oauth/token
  name: oAuth2
  sources:
  - openapi/confluence-cloud-v2.yml
  type: oauth2
- description: Personal Access Token or OAuth 2.0 Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/confluence-cloud-v2.yml
  type: http
slug: confluence-authentication
source_filename: confluence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/confluence-cloud-v2.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using email and API token. Provide your Atlassian account\n    email as the username and an API token as the password.\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/oauth/token\n    scopes: 9\n  description: OAuth 2.0 (3LO) for Confluence Cloud apps.\n  sources:\n  - openapi/confluence-cloud-v2.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal Access Token or OAuth 2.0 Bearer token.\n  sources:\n  - openapi/confluence-cloud-v2.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/authentication/confluence-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
---
