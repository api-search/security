---
anonymous_access: false
api_key_in: []
api_specs:
- filename: linkdigest-dev-capture-api-openapi.yml
  format: yaml
  label: LinkDigest Capture API
  slug: linkdigest-dev-capture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-capture-api-openapi.yml
- filename: linkdigest-dev-digest-api-openapi.yml
  format: yaml
  label: LinkDigest Digest API
  slug: linkdigest-dev-digest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-digest-api-openapi.yml
- filename: linkdigest-dev-health-api-openapi.yml
  format: yaml
  label: LinkDigest Health API
  slug: linkdigest-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-health-api-openapi.yml
- filename: linkdigest-dev-keys-api-openapi.yml
  format: yaml
  label: LinkDigest Keys API
  slug: linkdigest-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-keys-api-openapi.yml
- filename: linkdigest-dev-radar-api-openapi.yml
  format: yaml
  label: LinkDigest Radar API
  slug: linkdigest-dev-radar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-radar-api-openapi.yml
- filename: linkdigest-dev-search-api-openapi.yml
  format: yaml
  label: LinkDigest Search API
  slug: linkdigest-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-search-api-openapi.yml
- filename: linkdigest-dev-usage-api-openapi.yml
  format: yaml
  label: LinkDigest Usage API
  slug: linkdigest-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-usage-api-openapi.yml
- filename: linkdigest-dev-watch-api-openapi.yml
  format: yaml
  label: LinkDigest Watch API
  slug: linkdigest-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdigest-dev/openapi/linkdigest-dev-watch-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LinkDigest Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkDigest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LinkDigest
provider_slug: linkdigest-dev
scheme_count: 1
schemes:
- description: Your API key (ld_live_…) from https://linkdigest.dev/signin?ref=openapi&next=/app/keys.
  name: bearer
  scheme: bearer
  sources:
  - openapi/linkdigest-dev-openapi.json
  type: http
slug: linkdigest-dev-authentication
source_filename: linkdigest-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/linkdigest-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Your API key (ld_live_…) from https://linkdigest.dev/signin?ref=openapi&next=/app/keys.\n  sources:\n  - openapi/linkdigest-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/linkdigest-dev/authentication/linkdigest-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Social Media
- Data Extraction
- Search
- Content Aggregation
---
