---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: irmu-com-booking-api-openapi.yml
  format: yaml
  label: Irmu Booking API
  slug: irmu-com-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-booking-api-openapi.yml
- filename: irmu-com-crawl-api-openapi.yml
  format: yaml
  label: Irmu Crawl API
  slug: irmu-com-crawl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-crawl-api-openapi.yml
- filename: irmu-com-google-api-openapi.yml
  format: yaml
  label: Irmu Google API
  slug: irmu-com-google-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-google-api-openapi.yml
- filename: irmu-com-screenshot-api-openapi.yml
  format: yaml
  label: Irmu Screenshot API
  slug: irmu-com-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-screenshot-api-openapi.yml
- filename: irmu-com-chat-gpt-api-openapi.yml
  format: yaml
  label: Irmu Chat GPT API
  slug: irmu-com-chat-gpt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/irmu-com/openapi/irmu-com-chat-gpt-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Irmu Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Irmu secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Irmu
provider_slug: irmu-com
scheme_count: 2
schemes:
- description: '`Authorization: Bearer <key>`. The usual way in.'
  name: apiKeyHeader
  scheme: bearer
  sources:
  - openapi/app.irmu.com.yaml
  - openapi/irmu-com-openapi.yaml
  type: http
- description: '`?key=<key>`. Accepted on the crawl route only, and only when no

    `Authorization` header was sent.'
  in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/app.irmu.com.yaml
  - openapi/irmu-com-openapi.yaml
  type: apiKey
slug: irmu-com-authentication
source_filename: irmu-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/app.irmu.com.yaml, openapi/irmu-com-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyHeader\n  type: http\n  scheme: bearer\n  description: '`Authorization: Bearer <key>`. The usual way in.'\n  sources:\n  - openapi/app.irmu.com.yaml\n  - openapi/irmu-com-openapi.yaml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: |-\n    `?key=<key>`. Accepted on the crawl route only, and only when no\n    `Authorization` header was sent.\n  sources:\n  - openapi/app.irmu.com.yaml\n  - openapi/irmu-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/irmu-com/authentication/irmu-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Web Scraping
- Developer Tools
- Automation
- Data Extraction
- Company
---
