---
api_key_in: []
api_specs:
- filename: datocms-environments-api-openapi.yml
  format: yaml
  label: DatoCMS Environments API
  slug: datocms-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/openapi/datocms-environments-api-openapi.yml
- filename: datocms-fields-api-openapi.yml
  format: yaml
  label: DatoCMS Fields API
  slug: datocms-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/openapi/datocms-fields-api-openapi.yml
- filename: datocms-item-types-api-openapi.yml
  format: yaml
  label: DatoCMS Item Types API
  slug: datocms-item-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/openapi/datocms-item-types-api-openapi.yml
- filename: datocms-items-api-openapi.yml
  format: yaml
  label: DatoCMS Items API
  slug: datocms-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/openapi/datocms-items-api-openapi.yml
- filename: datocms-site-api-openapi.yml
  format: yaml
  label: DatoCMS Site API
  slug: datocms-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/openapi/datocms-site-api-openapi.yml
- filename: datocms-uploads-api-openapi.yml
  format: yaml
  label: DatoCMS Uploads API
  slug: datocms-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/openapi/datocms-uploads-api-openapi.yml
- filename: datocms-webhooks-api-openapi.yml
  format: yaml
  label: DatoCMS Webhooks API
  slug: datocms-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/openapi/datocms-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Datocms Authentication
name_suffix: Authentication
oauth_flows: []
overview: DatoCMS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DatoCMS
provider_slug: datocms
scheme_count: 1
schemes:
- bearerFormat: API token
  name: apiTokenAuth
  scheme: bearer
  sources:
  - openapi/datocms-content-management-api.yml
  type: http
slug: datocms-authentication
source_filename: datocms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datocms-content-management-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiTokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API token\n  sources:\n  - openapi/datocms-content-management-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/authentication/datocms-authentication.yml
summary_line: http · 1 scheme
tags:
- CMS
- Content Delivery
- Content Management
- GraphQL
- Headless CMS
---
