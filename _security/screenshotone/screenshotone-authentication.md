---
api_key_in:
- header
- query
api_specs:
- filename: screenshotone-openapi.yml
  format: yaml
  label: ScreenshotOne API
  slug: screenshotone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenshotone/refs/heads/main/openapi/screenshotone-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Screenshotone Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScreenshotOne secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ScreenshotOne
provider_slug: screenshotone
scheme_count: 2
schemes:
- description: API access key passed as a query string parameter.
  in: query
  name: accessKeyQuery
  parameter: access_key
  sources:
  - openapi/screenshotone-openapi.yml
  type: apiKey
- description: API access key passed via the X-Access-Key request header.
  in: header
  name: accessKeyHeader
  parameter: X-Access-Key
  sources:
  - openapi/screenshotone-openapi.yml
  type: apiKey
slug: screenshotone-authentication
source_filename: screenshotone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/screenshotone-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: accessKeyQuery\n  type: apiKey\n  in: query\n  parameter: access_key\n  description: API access key passed as a query string parameter.\n  sources:\n  - openapi/screenshotone-openapi.yml\n- name: accessKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Access-Key\n  description: API access key passed via the X-Access-Key request header.\n  sources:\n  - openapi/screenshotone-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/screenshotone/refs/heads/main/authentication/screenshotone-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Images
- Screenshots
- Web Rendering
---
