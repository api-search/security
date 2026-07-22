---
api_key_in: []
api_specs:
- filename: localytics-campaigns-audiences-openapi.yml
  format: yaml
  label: Localytics Campaigns And Audience API
  slug: localytics-campaigns-and-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/openapi/localytics-campaigns-audiences-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Localytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Localytics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Localytics
provider_slug: localytics
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/localytics-campaigns-audiences-openapi.yml
  type: http
slug: localytics-authentication
source_filename: localytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/localytics-campaigns-audiences-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/localytics-campaigns-audiences-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/authentication/localytics-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Martech
- Mobile Analytics
- Push Notifications
- Customer Engagement
- Marketing Automation
- APIs
---
