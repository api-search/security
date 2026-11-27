---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dnsdoctor-dev-domains-api-openapi.yml
  format: yaml
  label: DNS Doctor Domains API
  slug: dnsdoctor-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-domains-api-openapi.yml
- filename: dnsdoctor-dev-monitoring-api-openapi.yml
  format: yaml
  label: DNS Doctor Monitoring API
  slug: dnsdoctor-dev-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-monitoring-api-openapi.yml
- filename: dnsdoctor-dev-scan-api-openapi.yml
  format: yaml
  label: DNS Doctor Scan API
  slug: dnsdoctor-dev-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-scan-api-openapi.yml
- filename: dnsdoctor-dev-tools-api-openapi.yml
  format: yaml
  label: DNS Doctor Tools API
  slug: dnsdoctor-dev-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-tools-api-openapi.yml
- filename: dnsdoctor-dev-watch-api-openapi.yml
  format: yaml
  label: DNS Doctor Watch API
  slug: dnsdoctor-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-watch-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: DNS Doctor Authentication
name_suffix: Authentication
oauth_flows: []
overview: DNS Doctor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DNS Doctor
provider_slug: dnsdoctor-dev
scheme_count: 1
schemes:
- description: 'A DNS Doctor API token: `Authorization: Bearer dnsd_…`.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/dnsdoctor-dev-openapi.json
  type: http
slug: dnsdoctor-dev-authentication
source_filename: dnsdoctor-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/dnsdoctor-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'A DNS Doctor API token: `Authorization: Bearer dnsd_…`.'\n  sources:\n  - openapi/dnsdoctor-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dnsdoctor-dev/authentication/dnsdoctor-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- DNS
- DNS Tools
- Email Authentication
- Web Application
---
