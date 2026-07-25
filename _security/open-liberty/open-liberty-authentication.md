---
api_key_in: []
api_specs:
- filename: open-liberty-configuration-api-openapi.yml
  format: yaml
  label: Open Liberty Configuration API
  slug: open-liberty-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-liberty/refs/heads/main/openapi/open-liberty-configuration-api-openapi.yml
- filename: open-liberty-health-api-openapi.yml
  format: yaml
  label: Open Liberty Health API
  slug: open-liberty-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-liberty/refs/heads/main/openapi/open-liberty-health-api-openapi.yml
- filename: open-liberty-metrics-api-openapi.yml
  format: yaml
  label: Open Liberty Metrics API
  slug: open-liberty-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-liberty/refs/heads/main/openapi/open-liberty-metrics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Open Liberty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Liberty secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open Liberty
provider_slug: open-liberty
scheme_count: 1
schemes:
- description: Admin user credentials configured in server.xml.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/open-liberty-admin.json
  type: http
slug: open-liberty-authentication
source_filename: open-liberty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/open-liberty-admin.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Admin user credentials configured in server.xml.\n  sources:\n  - openapi/open-liberty-admin.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-liberty/refs/heads/main/authentication/open-liberty-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Server
- Cloud Native
- IBM
- Jakarta EE
- Java
- MicroProfile
- Microservices
---
