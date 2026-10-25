---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: openspace-custom-field-notes-api-openapi.yml
  format: yaml
  label: OpenSpace Custom Field Notes API
  slug: openspace-custom-field-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-custom-field-notes-api-openapi.yml
- filename: openspace-external-executive-view-controller-api-openapi.yml
  format: yaml
  label: OpenSpace External Executive View Controller API
  slug: openspace-external-executive-view-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-external-executive-view-controller-api-openapi.yml
- filename: openspace-field-notes-api-openapi.yml
  format: yaml
  label: OpenSpace Field notes API
  slug: openspace-field-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-field-notes-api-openapi.yml
- filename: openspace-global-config-api-openapi.yml
  format: yaml
  label: OpenSpace Global config API
  slug: openspace-global-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-global-config-api-openapi.yml
- filename: openspace-images-api-openapi.yml
  format: yaml
  label: OpenSpace Images API
  slug: openspace-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-images-api-openapi.yml
- filename: openspace-organizations-api-openapi.yml
  format: yaml
  label: OpenSpace Organizations API
  slug: openspace-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-organizations-api-openapi.yml
- filename: openspace-progress-tracking-api-openapi.yml
  format: yaml
  label: OpenSpace Progress Tracking API
  slug: openspace-progress-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-progress-tracking-api-openapi.yml
- filename: openspace-reports-api-openapi.yml
  format: yaml
  label: OpenSpace Reports API
  slug: openspace-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-reports-api-openapi.yml
- filename: openspace-sites-api-openapi.yml
  format: yaml
  label: OpenSpace Sites API
  slug: openspace-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-sites-api-openapi.yml
- filename: openspace-webhook-deliveries-api-openapi.yml
  format: yaml
  label: OpenSpace Webhook Deliveries API
  slug: openspace-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-webhook-deliveries-api-openapi.yml
- filename: openspace-webhook-headers-api-openapi.yml
  format: yaml
  label: OpenSpace Webhook Headers API
  slug: openspace-webhook-headers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-webhook-headers-api-openapi.yml
- filename: openspace-webhook-rules-api-openapi.yml
  format: yaml
  label: OpenSpace Webhook Rules API
  slug: openspace-webhook-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-webhook-rules-api-openapi.yml
- filename: openspace-webhooks-api-openapi.yml
  format: yaml
  label: OpenSpace Webhooks API
  slug: openspace-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Openspace Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenSpace secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenSpace
provider_slug: openspace
scheme_count: 2
schemes:
- in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/openspace-openapi.yml
  type: apiKey
- bearerFormat: jwt
  name: jwt-auth
  scheme: bearer
  sources:
  - openapi/openspace-openapi.yml
  type: http
slug: openspace-authentication
source_filename: openspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/openspace-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/openspace-openapi.yml\n- name: jwt-auth\n  type: http\n  scheme: bearer\n  bearerFormat: jwt\n  sources:\n  - openapi/openspace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/authentication/openspace-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Construction Technology
- Visual Intelligence
- 360 Camera
- Jobsite Documentation
- Progress Tracking
- BIM
- Drone Imagery
- Computer Vision
- Artificial Intelligence
- Software-as-a-Service
- San Francisco
---
