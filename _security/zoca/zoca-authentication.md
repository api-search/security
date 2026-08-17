---
api_key_in: []
api_specs:
- filename: zoca-platform-openapi.yml
  format: yaml
  label: Zoca Platform API
  slug: zoca-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/openapi/zoca-platform-openapi.yml
- filename: zoca-tasks-openapi.yml
  format: yaml
  label: Zoca Tasks API
  slug: zoca-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/openapi/zoca-tasks-openapi.yml
- filename: zoca-public-openapi.yml
  format: yaml
  label: Zoca Public API
  slug: zoca-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/openapi/zoca-public-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zoca Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zoca secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zoca
provider_slug: zoca
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter JWT token in the format Bearer <token>
  name: access-token
  scheme: bearer
  sources:
  - openapi/zoca-platform-openapi.yml
  - openapi/zoca-public-openapi.yml
  - openapi/zoca-tasks-openapi.yml
  type: http
slug: zoca-authentication
source_filename: zoca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/zoca-platform-openapi.yml, openapi/zoca-public-openapi.yml, openapi/zoca-tasks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: access-token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter JWT token in the format Bearer <token>\n  sources:\n  - openapi/zoca-platform-openapi.yml\n  - openapi/zoca-public-openapi.yml\n  - openapi/zoca-tasks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/authentication/zoca-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Marketing
- Beauty and Wellness
- Local Business
- AI Agents
- Appointments
- Scheduling
- Booking
- Local SEO
- Google Business Profile
- Social Media
- Salon Software
- Spa
- SaaS
- Lead Generation
- Customer Retention
- Small Business
---
