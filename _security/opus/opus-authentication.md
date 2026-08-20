---
api_key_in: []
api_specs:
- filename: opus-brand-templates-api-openapi.yml
  format: yaml
  label: Opus brand-templates API
  slug: opus-brand-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-brand-templates-api-openapi.yml
- filename: opus-censor-jobs-api-openapi.yml
  format: yaml
  label: Opus censor-jobs API
  slug: opus-censor-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-censor-jobs-api-openapi.yml
- filename: opus-clip-project-api-openapi.yml
  format: yaml
  label: Opus clip-project API
  slug: opus-clip-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-clip-project-api-openapi.yml
- filename: opus-collection-api-openapi.yml
  format: yaml
  label: Opus collection API
  slug: opus-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-collection-api-openapi.yml
- filename: opus-collection-content-api-openapi.yml
  format: yaml
  label: Opus collection-content API
  slug: opus-collection-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-collection-content-api-openapi.yml
- filename: opus-enterprise-api-openapi.yml
  format: yaml
  label: Opus enterprise API
  slug: opus-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-enterprise-api-openapi.yml
- filename: opus-exportable-clips-api-openapi.yml
  format: yaml
  label: Opus exportable-clips API
  slug: opus-exportable-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-exportable-clips-api-openapi.yml
- filename: opus-exportableclip-api-openapi.yml
  format: yaml
  label: Opus ExportableClip API
  slug: opus-exportableclip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-exportableclip-api-openapi.yml
- filename: opus-generative-jobs-api-openapi.yml
  format: yaml
  label: Opus generative-jobs API
  slug: opus-generative-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-generative-jobs-api-openapi.yml
- filename: opus-social-posting-api-openapi.yml
  format: yaml
  label: Opus social-posting API
  slug: opus-social-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-social-posting-api-openapi.yml
- filename: opus-transcripts-api-openapi.yml
  format: yaml
  label: Opus transcripts API
  slug: opus-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/openapi/opus-transcripts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Opus
provider_slug: opus
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/opus-openapi-original.json
  type: http
slug: opus-authentication
source_filename: opus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/opus-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/opus-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opus/refs/heads/main/authentication/opus-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Frontier Tech
- Video
- Artificial Intelligence
- Video Editing
- Short-Form Video
- Content Creation
- Social-Media
- Media
- Agents
---
