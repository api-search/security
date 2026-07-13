---
api_key_in:
- query
api_specs:
- filename: pagespeed-insights-openapi.yml
  format: yaml
  label: PageSpeed Insights API
  slug: pagespeed-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pagespeed/refs/heads/main/openapi/pagespeed-insights-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Google Pagespeed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google PageSpeed secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Google PageSpeed
provider_slug: google-pagespeed
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/pagespeed-insights-openapi.yml
  type: apiKey
slug: google-pagespeed-authentication
source_filename: google-pagespeed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pagespeed-insights-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/pagespeed-insights-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pagespeed/refs/heads/main/authentication/google-pagespeed-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Core Web Vitals
- Google
- Lighthouse
- Page Speed
- SEO
- Web Performance
---
