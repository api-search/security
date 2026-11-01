---
anonymous_access: false
api_key_in: []
api_specs:
- filename: majr-app-audit-api-openapi.yml
  format: yaml
  label: majr-app Audit API
  slug: majr-app-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-audit-api-openapi.yml
- filename: majr-app-discovery-api-openapi.yml
  format: yaml
  label: majr-app Discovery API
  slug: majr-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-discovery-api-openapi.yml
- filename: majr-app-drafting-api-openapi.yml
  format: yaml
  label: majr-app Drafting API
  slug: majr-app-drafting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-drafting-api-openapi.yml
- filename: majr-app-encode-api-openapi.yml
  format: yaml
  label: majr-app Encode API
  slug: majr-app-encode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-encode-api-openapi.yml
- filename: majr-app-generation-api-openapi.yml
  format: yaml
  label: majr-app Generation API
  slug: majr-app-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-generation-api-openapi.yml
- filename: majr-app-healthz-api-openapi.yml
  format: yaml
  label: majr-app Healthz API
  slug: majr-app-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-healthz-api-openapi.yml
- filename: majr-app-jobs-api-openapi.yml
  format: yaml
  label: majr-app Jobs API
  slug: majr-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-jobs-api-openapi.yml
- filename: majr-app-uploads-api-openapi.yml
  format: yaml
  label: majr-app Uploads API
  slug: majr-app-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-uploads-api-openapi.yml
- filename: majr-app-usage-api-openapi.yml
  format: yaml
  label: majr-app Usage API
  slug: majr-app-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-usage-api-openapi.yml
- filename: majr-app-voice-api-openapi.yml
  format: yaml
  label: majr-app Voice API
  slug: majr-app-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-voice-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Majr App Authentication
name_suffix: Authentication
oauth_flows: []
overview: majr-app secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: majr-app
provider_slug: majr-app
scheme_count: 1
schemes:
- description: Service API key (`rn_...`), minted per product on the platform Control Plane.
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/dispatch-openapi.json
  - openapi/encoding-openapi.json
  - openapi/seo-openapi.json
  type: http
slug: majr-app-authentication
source_filename: majr-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/dispatch-openapi.json, openapi/encoding-openapi.json, openapi/seo-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: Service API key (`rn_...`), minted per product on the platform Control Plane.\n  sources:\n  - openapi/dispatch-openapi.json\n  - openapi/encoding-openapi.json\n  - openapi/seo-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/majr-app/authentication/majr-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Media
- SEO
- Encoding
- Agent Services
---
