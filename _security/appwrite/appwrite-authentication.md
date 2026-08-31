---
api_key_in:
- header
api_specs:
- filename: appwrite-account-api-openapi.yml
  format: yaml
  label: Appwrite Account API
  slug: appwrite-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/openapi/appwrite-account-api-openapi.yml
- filename: appwrite-databases-api-openapi.yml
  format: yaml
  label: Appwrite Databases API
  slug: appwrite-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/openapi/appwrite-databases-api-openapi.yml
- filename: appwrite-storage-api-openapi.yml
  format: yaml
  label: Appwrite Storage API
  slug: appwrite-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/openapi/appwrite-storage-api-openapi.yml
- filename: appwrite-users-api-openapi.yml
  format: yaml
  label: Appwrite Users API
  slug: appwrite-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/openapi/appwrite-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Appwrite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appwrite secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appwrite
provider_slug: appwrite
scheme_count: 1
schemes:
- in: header
  name: projectKey
  parameter: X-Appwrite-Project
  sources:
  - openapi/appwrite-openapi.yaml
  type: apiKey
slug: appwrite-authentication
source_filename: appwrite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appwrite-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: projectKey\n  type: apiKey\n  in: header\n  parameter: X-Appwrite-Project\n  sources:\n  - openapi/appwrite-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/authentication/appwrite-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Application
- Backends
- Mobile
- Open-Source
---
