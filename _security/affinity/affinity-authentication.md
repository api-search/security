---
api_key_in: []
api_specs:
- filename: affinity-auth-api-openapi.yml
  format: yaml
  label: Affinity auth API
  slug: affinity-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-auth-api-openapi.yml
- filename: affinity-companies-api-openapi.yml
  format: yaml
  label: Affinity companies API
  slug: affinity-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-companies-api-openapi.yml
- filename: affinity-companymerges-api-openapi.yml
  format: yaml
  label: Affinity companyMerges API
  slug: affinity-companymerges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-companymerges-api-openapi.yml
- filename: affinity-emails-api-openapi.yml
  format: yaml
  label: Affinity emails API
  slug: affinity-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-emails-api-openapi.yml
- filename: affinity-lists-api-openapi.yml
  format: yaml
  label: Affinity lists API
  slug: affinity-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-lists-api-openapi.yml
- filename: affinity-meetings-api-openapi.yml
  format: yaml
  label: Affinity meetings API
  slug: affinity-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-meetings-api-openapi.yml
- filename: affinity-notes-api-openapi.yml
  format: yaml
  label: Affinity notes API
  slug: affinity-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-notes-api-openapi.yml
- filename: affinity-opportunities-api-openapi.yml
  format: yaml
  label: Affinity opportunities API
  slug: affinity-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-opportunities-api-openapi.yml
- filename: affinity-personmerges-api-openapi.yml
  format: yaml
  label: Affinity personMerges API
  slug: affinity-personmerges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-personmerges-api-openapi.yml
- filename: affinity-persons-api-openapi.yml
  format: yaml
  label: Affinity persons API
  slug: affinity-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/openapi/affinity-persons-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Affinity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Affinity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Affinity
provider_slug: affinity
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/affinity-v2-openapi.yml
  type: http
slug: affinity-authentication
source_filename: affinity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/affinity-v2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/affinity-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinity/refs/heads/main/authentication/affinity-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Relationship Intelligence
- Private Equity
- Venture Capital
- Contacts
- Organization
- Opportunities
- Deal Management
---
