---
api_key_in: []
api_specs:
- filename: wikimedia-articles-api-openapi.yml
  format: yaml
  label: Wikimedia articles API
  slug: wikimedia-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-articles-api-openapi.yml
- filename: wikimedia-batches-api-openapi.yml
  format: yaml
  label: Wikimedia batches API
  slug: wikimedia-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-batches-api-openapi.yml
- filename: wikimedia-citation-api-openapi.yml
  format: yaml
  label: Wikimedia Citation API
  slug: wikimedia-citation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-citation-api-openapi.yml
- filename: wikimedia-codes-api-openapi.yml
  format: yaml
  label: Wikimedia codes API
  slug: wikimedia-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-codes-api-openapi.yml
- filename: wikimedia-languages-api-openapi.yml
  format: yaml
  label: Wikimedia languages API
  slug: wikimedia-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-languages-api-openapi.yml
- filename: wikimedia-math-api-openapi.yml
  format: yaml
  label: Wikimedia Math API
  slug: wikimedia-math-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-math-api-openapi.yml
- filename: wikimedia-mobile-api-openapi.yml
  format: yaml
  label: Wikimedia Mobile API
  slug: wikimedia-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-mobile-api-openapi.yml
- filename: wikimedia-namespaces-api-openapi.yml
  format: yaml
  label: Wikimedia namespaces API
  slug: wikimedia-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-namespaces-api-openapi.yml
- filename: wikimedia-offline-api-openapi.yml
  format: yaml
  label: Wikimedia offline API
  slug: wikimedia-offline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-offline-api-openapi.yml
- filename: wikimedia-page-content-api-openapi.yml
  format: yaml
  label: Wikimedia Page content API
  slug: wikimedia-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-page-content-api-openapi.yml
- filename: wikimedia-projects-api-openapi.yml
  format: yaml
  label: Wikimedia projects API
  slug: wikimedia-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-projects-api-openapi.yml
- filename: wikimedia-reading-lists-api-openapi.yml
  format: yaml
  label: Wikimedia Reading lists API
  slug: wikimedia-reading-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-reading-lists-api-openapi.yml
- filename: wikimedia-recommendation-api-openapi.yml
  format: yaml
  label: Wikimedia Recommendation API
  slug: wikimedia-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-recommendation-api-openapi.yml
- filename: wikimedia-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia snapshots API
  slug: wikimedia-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-snapshots-api-openapi.yml
- filename: wikimedia-structured-contents-api-openapi.yml
  format: yaml
  label: Wikimedia structured-contents API
  slug: wikimedia-structured-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-structured-contents-api-openapi.yml
- filename: wikimedia-structured-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia structured-snapshots API
  slug: wikimedia-structured-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-structured-snapshots-api-openapi.yml
- filename: wikimedia-talk-pages-api-openapi.yml
  format: yaml
  label: Wikimedia Talk pages API
  slug: wikimedia-talk-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-talk-pages-api-openapi.yml
- filename: wikimedia-transforms-api-openapi.yml
  format: yaml
  label: Wikimedia Transforms API
  slug: wikimedia-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-transforms-api-openapi.yml
- filename: wikimedia-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia wikidata API
  slug: wikimedia-wikidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-wikidata-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wikimedia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wikimedia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wikimedia
provider_slug: wikimedia
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wikimedia-enterprise-api.yaml
  type: http
slug: wikimedia-authentication
source_filename: wikimedia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wikimedia-enterprise-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/wikimedia-enterprise-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/authentication/wikimedia-authentication.yml
summary_line: http · 1 scheme
tags:
- Wikipedia
- Wikimedia
- Encyclopedia
- Open Knowledge
- Content
- Search
- Reference
---
