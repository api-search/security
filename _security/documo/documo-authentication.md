---
api_key_in: []
api_specs:
- filename: documo-openapi.yml
  format: yaml
  label: Documo Fax API
  slug: fax
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documo/refs/heads/main/openapi/documo-openapi.yml
- filename: documo-openapi.yml
  format: yaml
  label: Documo Numbers API
  slug: numbers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documo/refs/heads/main/openapi/documo-openapi.yml
- filename: documo-openapi.yml
  format: yaml
  label: Documo Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documo/refs/heads/main/openapi/documo-openapi.yml
- filename: documo-openapi.yml
  format: yaml
  label: Documo Account API
  slug: account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/documo/refs/heads/main/openapi/documo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Documo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Documo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Documo
provider_slug: documo
scheme_count: 1
schemes:
- description: 'API key generated in the Documo web app under Settings > API. The key is sent in the Authorization header. Documo documents this as `Authorization: Basic <API_KEY>`, where the API key itself acts as the bearer credential. Each key carries an admin or user access level that determines which endpoints it may call.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/documo-openapi.yml
  type: http
slug: documo-authentication
source_filename: documo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/documo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'API key generated in the Documo web app under Settings > API. The key is sent\n    in the Authorization header. Documo documents this as `Authorization: Basic <API_KEY>`,\n    where the API key itself acts as the bearer credential. Each key carries an admin or user\n    access level that determines which endpoints it may call.'\n  sources:\n  - openapi/documo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/documo/refs/heads/main/authentication/documo-authentication.yml
summary_line: http · 1 scheme
tags:
- Fax
- Cloud Fax
- Document Delivery
- HIPAA
- Communications
---
