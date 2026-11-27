---
anonymous_access: false
api_key_in: []
api_specs:
- filename: katto-tech-brand-kit-api-openapi.yml
  format: yaml
  label: Katto Brand Kit API
  slug: katto-tech-brand-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/katto-tech/openapi/katto-tech-brand-kit-api-openapi.yml
- filename: katto-tech-connections-api-openapi.yml
  format: yaml
  label: Katto Connections API
  slug: katto-tech-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/katto-tech/openapi/katto-tech-connections-api-openapi.yml
- filename: katto-tech-jobs-api-openapi.yml
  format: yaml
  label: Katto Jobs API
  slug: katto-tech-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/katto-tech/openapi/katto-tech-jobs-api-openapi.yml
- filename: katto-tech-me-api-openapi.yml
  format: yaml
  label: Katto Me API
  slug: katto-tech-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/katto-tech/openapi/katto-tech-me-api-openapi.yml
- filename: katto-tech-scheduled-posts-api-openapi.yml
  format: yaml
  label: Katto Scheduled Posts API
  slug: katto-tech-scheduled-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/katto-tech/openapi/katto-tech-scheduled-posts-api-openapi.yml
- filename: katto-tech-uploads-api-openapi.yml
  format: yaml
  label: Katto Uploads API
  slug: katto-tech-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/katto-tech/openapi/katto-tech-uploads-api-openapi.yml
- filename: katto-tech-usage-api-openapi.yml
  format: yaml
  label: Katto Usage API
  slug: katto-tech-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/katto-tech/openapi/katto-tech-usage-api-openapi.yml
- filename: katto-tech-webhook-api-openapi.yml
  format: yaml
  label: Katto Webhook API
  slug: katto-tech-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/katto-tech/openapi/katto-tech-webhook-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Katto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Katto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Katto
provider_slug: katto-tech
scheme_count: 1
schemes:
- description: 'API key created at https://katto.tech/dashboard/api-keys, sent as `Authorization: Bearer sk_live_...`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/katto-tech-openapi.json
  type: http
slug: katto-tech-authentication
source_filename: katto-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/katto-tech-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key created at https://katto.tech/dashboard/api-keys, sent as `Authorization:\n    Bearer sk_live_...`.'\n  sources:\n  - openapi/katto-tech-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/katto-tech/authentication/katto-tech-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Video
- Clip
- Social Media
- Software-as-a-Service
---
