---
api_key_in:
- header
- query
api_specs:
- filename: redmine-attachments-api-openapi.yml
  format: yaml
  label: Redmine Attachments API
  slug: redmine-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-attachments-api-openapi.yml
- filename: redmine-custom-fields-json-api-openapi.yml
  format: yaml
  label: Redmine Custom Fields.json API
  slug: redmine-custom-fields-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-custom-fields-json-api-openapi.yml
- filename: redmine-groups-json-api-openapi.yml
  format: yaml
  label: Redmine Groups.json API
  slug: redmine-groups-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-groups-json-api-openapi.yml
- filename: redmine-issue-statuses-json-api-openapi.yml
  format: yaml
  label: Redmine Issue Statuses.json API
  slug: redmine-issue-statuses-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-issue-statuses-json-api-openapi.yml
- filename: redmine-issues-api-openapi.yml
  format: yaml
  label: Redmine Issues API
  slug: redmine-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-issues-api-openapi.yml
- filename: redmine-issues-json-api-openapi.yml
  format: yaml
  label: Redmine Issues.json API
  slug: redmine-issues-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-issues-json-api-openapi.yml
- filename: redmine-my-api-openapi.yml
  format: yaml
  label: Redmine My API
  slug: redmine-my-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-my-api-openapi.yml
- filename: redmine-projects-api-openapi.yml
  format: yaml
  label: Redmine Projects API
  slug: redmine-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-projects-api-openapi.yml
- filename: redmine-projects-json-api-openapi.yml
  format: yaml
  label: Redmine Projects.json API
  slug: redmine-projects-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-projects-json-api-openapi.yml
- filename: redmine-roles-json-api-openapi.yml
  format: yaml
  label: Redmine Roles.json API
  slug: redmine-roles-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-roles-json-api-openapi.yml
- filename: redmine-time-entries-api-openapi.yml
  format: yaml
  label: Redmine Time Entries API
  slug: redmine-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-time-entries-api-openapi.yml
- filename: redmine-time-entries-json-api-openapi.yml
  format: yaml
  label: Redmine Time Entries.json API
  slug: redmine-time-entries-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-time-entries-json-api-openapi.yml
- filename: redmine-trackers-json-api-openapi.yml
  format: yaml
  label: Redmine Trackers.json API
  slug: redmine-trackers-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-trackers-json-api-openapi.yml
- filename: redmine-uploads-json-api-openapi.yml
  format: yaml
  label: Redmine Uploads.json API
  slug: redmine-uploads-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-uploads-json-api-openapi.yml
- filename: redmine-users-api-openapi.yml
  format: yaml
  label: Redmine Users API
  slug: redmine-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-users-api-openapi.yml
- filename: redmine-users-json-api-openapi.yml
  format: yaml
  label: Redmine Users.json API
  slug: redmine-users-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-users-json-api-openapi.yml
- filename: redmine-wiki-pages-json-api-openapi.yml
  format: yaml
  label: Redmine Wiki Pages.json API
  slug: redmine-wiki-pages-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-wiki-pages-json-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Redmine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Redmine secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Redmine
provider_slug: redmine
scheme_count: 3
schemes:
- in: header
  name: apiKeyHeader
  parameter: X-Redmine-API-Key
  sources:
  - openapi/redmine-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/redmine-openapi.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/redmine-openapi.yml
  type: http
slug: redmine-authentication
source_filename: redmine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/redmine-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Redmine-API-Key\n  sources:\n  - openapi/redmine-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/redmine-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/redmine-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/authentication/redmine-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Project Management
- Issue Tracking
- Open-Source
- Ruby on Rails
- Bug Tracking
- Time Tracking
---
