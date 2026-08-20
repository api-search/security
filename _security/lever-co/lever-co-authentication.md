---
api_key_in: []
api_specs:
- filename: lever-webhooks-asyncapi.yml
  format: yaml
  label: Lever Webhooks
  slug: lever-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-webhooks-asyncapi.yml
- filename: lever-co-applications-api-openapi.yml
  format: yaml
  label: Lever Applications API
  slug: lever-co-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-applications-api-openapi.yml
- filename: lever-co-archive-reasons-api-openapi.yml
  format: yaml
  label: Lever Archive Reasons API
  slug: lever-co-archive-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-archive-reasons-api-openapi.yml
- filename: lever-co-audit-events-api-openapi.yml
  format: yaml
  label: Lever Audit Events API
  slug: lever-co-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-audit-events-api-openapi.yml
- filename: lever-co-eeo-responses-api-openapi.yml
  format: yaml
  label: Lever EEO Responses API
  slug: lever-co-eeo-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-eeo-responses-api-openapi.yml
- filename: lever-co-feedback-api-openapi.yml
  format: yaml
  label: Lever Feedback API
  slug: lever-co-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-feedback-api-openapi.yml
- filename: lever-co-files-api-openapi.yml
  format: yaml
  label: Lever Files API
  slug: lever-co-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-files-api-openapi.yml
- filename: lever-co-interviews-api-openapi.yml
  format: yaml
  label: Lever Interviews API
  slug: lever-co-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-interviews-api-openapi.yml
- filename: lever-co-notes-api-openapi.yml
  format: yaml
  label: Lever Notes API
  slug: lever-co-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-notes-api-openapi.yml
- filename: lever-co-offers-api-openapi.yml
  format: yaml
  label: Lever Offers API
  slug: lever-co-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-offers-api-openapi.yml
- filename: lever-co-opportunities-api-openapi.yml
  format: yaml
  label: Lever Opportunities API
  slug: lever-co-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-opportunities-api-openapi.yml
- filename: lever-co-panels-api-openapi.yml
  format: yaml
  label: Lever Panels API
  slug: lever-co-panels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-panels-api-openapi.yml
- filename: lever-co-postings-api-openapi.yml
  format: yaml
  label: Lever Postings API
  slug: lever-co-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-postings-api-openapi.yml
- filename: lever-co-requisitions-api-openapi.yml
  format: yaml
  label: Lever Requisitions API
  slug: lever-co-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-requisitions-api-openapi.yml
- filename: lever-co-sources-api-openapi.yml
  format: yaml
  label: Lever Sources API
  slug: lever-co-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-sources-api-openapi.yml
- filename: lever-co-stages-api-openapi.yml
  format: yaml
  label: Lever Stages API
  slug: lever-co-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-stages-api-openapi.yml
- filename: lever-co-tags-api-openapi.yml
  format: yaml
  label: Lever Tags API
  slug: lever-co-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-tags-api-openapi.yml
- filename: lever-co-users-api-openapi.yml
  format: yaml
  label: Lever Users API
  slug: lever-co-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-users-api-openapi.yml
- filename: lever-co-webhooks-api-openapi.yml
  format: yaml
  label: Lever Webhooks API
  slug: lever-co-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lever Co Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lever secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lever
provider_slug: lever-co
scheme_count: 2
schemes:
- description: HTTP Basic authentication using a Lever API key as the username and an empty password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/lever-data-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://auth.lever.co/authorize
    flow: authorizationCode
    scopes: 22
    tokenUrl: https://auth.lever.co/oauth/token
  name: OAuth2
  sources:
  - openapi/lever-data-api-openapi.yml
  type: oauth2
slug: lever-co-authentication
source_filename: lever-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lever-data-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using a Lever API key as the username and an empty\n    password.\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.lever.co/authorize\n    tokenUrl: https://auth.lever.co/oauth/token\n    scopes: 22\n  sources:\n  - openapi/lever-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/authentication/lever-co-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Applicant Tracking
- ATS
- CRM
- Recruiting
- Hiring
- Talent Acquisition
- Human Resources
- HR Tech
- Postings
- Webhook
- Authentication
---
