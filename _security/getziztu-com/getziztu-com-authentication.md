---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: getziztu-com-characters-api-openapi.yml
  format: yaml
  label: getziztu-com Characters API
  slug: getziztu-com-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-characters-api-openapi.yml
- filename: getziztu-com-credits-api-openapi.yml
  format: yaml
  label: getziztu-com Credits API
  slug: getziztu-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-credits-api-openapi.yml
- filename: getziztu-com-director-api-openapi.yml
  format: yaml
  label: getziztu-com Director API
  slug: getziztu-com-director-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-director-api-openapi.yml
- filename: getziztu-com-export-api-openapi.yml
  format: yaml
  label: getziztu-com Export API
  slug: getziztu-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-export-api-openapi.yml
- filename: getziztu-com-generate-api-openapi.yml
  format: yaml
  label: getziztu-com Generate API
  slug: getziztu-com-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-generate-api-openapi.yml
- filename: getziztu-com-jobs-api-openapi.yml
  format: yaml
  label: getziztu-com Jobs API
  slug: getziztu-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-jobs-api-openapi.yml
- filename: getziztu-com-media-api-openapi.yml
  format: yaml
  label: getziztu-com Media API
  slug: getziztu-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-media-api-openapi.yml
- filename: getziztu-com-meta-api-openapi.yml
  format: yaml
  label: getziztu-com Meta API
  slug: getziztu-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-meta-api-openapi.yml
- filename: getziztu-com-music-api-openapi.yml
  format: yaml
  label: getziztu-com Music API
  slug: getziztu-com-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-music-api-openapi.yml
- filename: getziztu-com-places-api-openapi.yml
  format: yaml
  label: getziztu-com Places API
  slug: getziztu-com-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-places-api-openapi.yml
- filename: getziztu-com-projects-api-openapi.yml
  format: yaml
  label: getziztu-com Projects API
  slug: getziztu-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-projects-api-openapi.yml
- filename: getziztu-com-script-api-openapi.yml
  format: yaml
  label: getziztu-com Script API
  slug: getziztu-com-script-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-script-api-openapi.yml
- filename: getziztu-com-shots-api-openapi.yml
  format: yaml
  label: getziztu-com Shots API
  slug: getziztu-com-shots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-shots-api-openapi.yml
- filename: getziztu-com-tools-api-openapi.yml
  format: yaml
  label: getziztu-com Tools API
  slug: getziztu-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-tools-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Getziztu Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: getziztu-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: getziztu-com
provider_slug: getziztu-com
scheme_count: 2
schemes:
- description: 'SaaS: Authorization: Bearer sk_sakuga_... | Local: Authorization: Bearer $SAKUGA_API_TOKEN'
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/getziztu-com-openapi.json
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/getziztu-com-openapi.json
  type: apiKey
slug: getziztu-com-authentication
source_filename: getziztu-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/getziztu-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: 'SaaS: Authorization: Bearer sk_sakuga_... | Local: Authorization: Bearer $SAKUGA_API_TOKEN'\n  sources:\n  - openapi/getziztu-com-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/getziztu-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getziztu-com/authentication/getziztu-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- AI
- Video
- SocialMedia
- ContentCreation
---
