---
api_key_in:
- header
api_specs:
- filename: escape-asm-api-openapi.yml
  format: yaml
  label: Escape Asm API
  slug: escape-asm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-asm-api-openapi.yml
- filename: escape-assets-api-openapi.yml
  format: yaml
  label: Escape Assets API
  slug: escape-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-assets-api-openapi.yml
- filename: escape-audit-api-openapi.yml
  format: yaml
  label: Escape Audit API
  slug: escape-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-audit-api-openapi.yml
- filename: escape-beta-api-openapi.yml
  format: yaml
  label: Escape Beta API
  slug: escape-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-beta-api-openapi.yml
- filename: escape-customrules-api-openapi.yml
  format: yaml
  label: Escape CustomRules API
  slug: escape-customrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-customrules-api-openapi.yml
- filename: escape-emails-api-openapi.yml
  format: yaml
  label: Escape Emails API
  slug: escape-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-emails-api-openapi.yml
- filename: escape-events-api-openapi.yml
  format: yaml
  label: Escape Events API
  slug: escape-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-events-api-openapi.yml
- filename: escape-integrations-api-openapi.yml
  format: yaml
  label: Escape Integrations API
  slug: escape-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-integrations-api-openapi.yml
- filename: escape-issues-api-openapi.yml
  format: yaml
  label: Escape Issues API
  slug: escape-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-issues-api-openapi.yml
- filename: escape-jobs-api-openapi.yml
  format: yaml
  label: Escape Jobs API
  slug: escape-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-jobs-api-openapi.yml
- filename: escape-locations-api-openapi.yml
  format: yaml
  label: Escape Locations API
  slug: escape-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-locations-api-openapi.yml
- filename: escape-profiles-api-openapi.yml
  format: yaml
  label: Escape Profiles API
  slug: escape-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-profiles-api-openapi.yml
- filename: escape-projects-api-openapi.yml
  format: yaml
  label: Escape Projects API
  slug: escape-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-projects-api-openapi.yml
- filename: escape-roles-api-openapi.yml
  format: yaml
  label: Escape Roles API
  slug: escape-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-roles-api-openapi.yml
- filename: escape-scans-api-openapi.yml
  format: yaml
  label: Escape Scans API
  slug: escape-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-scans-api-openapi.yml
- filename: escape-statistics-api-openapi.yml
  format: yaml
  label: Escape Statistics API
  slug: escape-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-statistics-api-openapi.yml
- filename: escape-tags-api-openapi.yml
  format: yaml
  label: Escape Tags API
  slug: escape-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-tags-api-openapi.yml
- filename: escape-upload-api-openapi.yml
  format: yaml
  label: Escape Upload API
  slug: escape-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-upload-api-openapi.yml
- filename: escape-users-api-openapi.yml
  format: yaml
  label: Escape Users API
  slug: escape-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-users-api-openapi.yml
- filename: escape-workflows-api-openapi.yml
  format: yaml
  label: Escape Workflows API
  slug: escape-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Escape Authentication
name_suffix: Authentication
oauth_flows: []
overview: Escape secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Escape
provider_slug: escape
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-ESCAPE-API-KEY
  sources:
  - openapi/escape-openapi.yml
  type: apiKey
slug: escape-authentication
source_filename: escape-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/escape-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-ESCAPE-API-KEY\n  sources:\n  - openapi/escape-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/authentication/escape-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Platform
- Security
---
