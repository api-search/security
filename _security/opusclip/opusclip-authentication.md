---
api_key_in: []
api_specs:
- filename: opusclip-brand-templates-api-openapi.yml
  format: yaml
  label: OpusClip brand-templates API
  slug: opusclip-brand-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-brand-templates-api-openapi.yml
- filename: opusclip-censor-jobs-api-openapi.yml
  format: yaml
  label: OpusClip censor-jobs API
  slug: opusclip-censor-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-censor-jobs-api-openapi.yml
- filename: opusclip-clip-project-api-openapi.yml
  format: yaml
  label: OpusClip clip-project API
  slug: opusclip-clip-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-clip-project-api-openapi.yml
- filename: opusclip-collection-api-openapi.yml
  format: yaml
  label: OpusClip collection API
  slug: opusclip-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-collection-api-openapi.yml
- filename: opusclip-collection-content-api-openapi.yml
  format: yaml
  label: OpusClip collection-content API
  slug: opusclip-collection-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-collection-content-api-openapi.yml
- filename: opusclip-enterprise-api-openapi.yml
  format: yaml
  label: OpusClip enterprise API
  slug: opusclip-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-enterprise-api-openapi.yml
- filename: opusclip-exportable-clips-api-openapi.yml
  format: yaml
  label: OpusClip exportable-clips API
  slug: opusclip-exportable-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-exportable-clips-api-openapi.yml
- filename: opusclip-exportableclip-api-openapi.yml
  format: yaml
  label: OpusClip ExportableClip API
  slug: opusclip-exportableclip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-exportableclip-api-openapi.yml
- filename: opusclip-generative-jobs-api-openapi.yml
  format: yaml
  label: OpusClip generative-jobs API
  slug: opusclip-generative-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-generative-jobs-api-openapi.yml
- filename: opusclip-social-posting-api-openapi.yml
  format: yaml
  label: OpusClip social-posting API
  slug: opusclip-social-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-social-posting-api-openapi.yml
- filename: opusclip-transcripts-api-openapi.yml
  format: yaml
  label: OpusClip transcripts API
  slug: opusclip-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-transcripts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Opusclip Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpusClip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpusClip
provider_slug: opusclip
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/opusclip-openapi-original.json
  type: http
slug: opusclip-authentication
source_filename: opusclip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/opusclip-openapi-original.json\ndocs: https://help.opus.pro/api-reference/overview\nsummary:\n  types:\n  - http\n  scheme: HTTP Bearer token; the API key is a JWT-format value passed as a Bearer token\n  header: 'Authorization: Bearer <API_KEY>'\n  org_header: 'x-opus-org-id: <ORG_ID> (required on some endpoints)'\n  key_source: OpusClip dashboard (https://clip.opus.pro/dashboard); Enterprise/Pro(Beta)/Max plans\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/opusclip-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/authentication/opusclip-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Video
- AI
- Video Editing
- Short-Form Video
- Social Media
- Content Creation
- MCP
- Developer API
---
