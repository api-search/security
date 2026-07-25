---
api_key_in:
- query
api_specs:
- filename: lilt-create-api-openapi.yml
  format: yaml
  label: Lilt Create API
  slug: lilt-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-create-api-openapi.yml
- filename: lilt-documents-api-openapi.yml
  format: yaml
  label: Lilt Documents API
  slug: lilt-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-documents-api-openapi.yml
- filename: lilt-domains-api-openapi.yml
  format: yaml
  label: Lilt Domains API
  slug: lilt-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-domains-api-openapi.yml
- filename: lilt-files-api-openapi.yml
  format: yaml
  label: Lilt Files API
  slug: lilt-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-files-api-openapi.yml
- filename: lilt-jobs-api-openapi.yml
  format: yaml
  label: Lilt Jobs API
  slug: lilt-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-jobs-api-openapi.yml
- filename: lilt-languages-api-openapi.yml
  format: yaml
  label: Lilt Languages API
  slug: lilt-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-languages-api-openapi.yml
- filename: lilt-memories-api-openapi.yml
  format: yaml
  label: Lilt Memories API
  slug: lilt-memories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-memories-api-openapi.yml
- filename: lilt-projects-api-openapi.yml
  format: yaml
  label: Lilt Projects API
  slug: lilt-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-projects-api-openapi.yml
- filename: lilt-segments-api-openapi.yml
  format: yaml
  label: Lilt Segments API
  slug: lilt-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-segments-api-openapi.yml
- filename: lilt-translate-api-openapi.yml
  format: yaml
  label: Lilt Translate API
  slug: lilt-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-translate-api-openapi.yml
- filename: lilt-uploads-api-openapi.yml
  format: yaml
  label: Lilt Uploads API
  slug: lilt-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-uploads-api-openapi.yml
- filename: lilt-webhook-configuration-api-openapi.yml
  format: yaml
  label: Lilt Webhook Configuration API
  slug: lilt-webhook-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-webhook-configuration-api-openapi.yml
- filename: lilt-workflows-api-openapi.yml
  format: yaml
  label: Lilt Workflows API
  slug: lilt-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-workflows-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lilt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lilt secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lilt
provider_slug: lilt
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/lilt-openapi-original.yml
  type: http
- in: query
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/lilt-openapi-original.yml
  type: apiKey
slug: lilt-authentication
source_filename: lilt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/lilt-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/lilt-openapi-original.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/lilt-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/authentication/lilt-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai
- Translation
- Localization
- Machine Translation
- Language
- Content
- Translation Memory
- Agents
---
