---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mentionry-com-actions-api-openapi.yml
  format: yaml
  label: Mentionry Actions API
  slug: mentionry-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionry-com/openapi/mentionry-com-actions-api-openapi.yml
- filename: mentionry-com-brand-api-openapi.yml
  format: yaml
  label: Mentionry Brand API
  slug: mentionry-com-brand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionry-com/openapi/mentionry-com-brand-api-openapi.yml
- filename: mentionry-com-deployments-api-openapi.yml
  format: yaml
  label: Mentionry Deployments API
  slug: mentionry-com-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionry-com/openapi/mentionry-com-deployments-api-openapi.yml
- filename: mentionry-com-jobs-api-openapi.yml
  format: yaml
  label: Mentionry Jobs API
  slug: mentionry-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionry-com/openapi/mentionry-com-jobs-api-openapi.yml
- filename: mentionry-com-reviews-api-openapi.yml
  format: yaml
  label: Mentionry Reviews API
  slug: mentionry-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionry-com/openapi/mentionry-com-reviews-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mentionry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mentionry secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mentionry
provider_slug: mentionry-com
scheme_count: 1
schemes:
- description: Dashboard-issued Mentionry key. New keys expire and are scoped to the selected brand. Saved insights allows reads; Page optimization adds action/job/deployment operations; Research and agents adds legacy research tools. Keys never bypass subscription limits. Expired/revoked credentials return 401; insufficient operation permission returns 403.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/mentionry-com-openapi.json
  type: http
slug: mentionry-com-authentication
source_filename: mentionry-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mentionry-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Dashboard-issued Mentionry key. New keys expire and are scoped to the selected\n    brand. Saved insights allows reads; Page optimization adds action/job/deployment operations;\n    Research and agents adds legacy research tools. Keys never bypass subscription limits. Expired/revoked\n    credentials return 401; insufficient operation permission returns 403.\n  sources:\n  - openapi/mentionry-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mentionry-com/authentication/mentionry-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- SEO
- Marketing
- Visibility
- Analytics
---
