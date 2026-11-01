---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: The Water Hub API
  slug: thewaterhub-api
  spec_type: OpenAPI
  url: https://thewaterhub.org/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Thewaterhub Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: thewaterhub-org declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: thewaterhub-org
provider_slug: thewaterhub-org
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  type: http
slug: thewaterhub-org-authentication
source_filename: thewaterhub-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://thewaterhub.org/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.\"\n    name: accessKey"
source_yaml_url: https://artifacts.apis.io/thewaterhub-org/authentication/thewaterhub-org-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Water
- Pricing
- Dataset
- API
---
