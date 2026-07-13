---
api_key_in: []
api_specs:
- filename: formant-admin-api.yaml
  format: yaml
  label: Formant Admin API
  slug: formant-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formant/refs/heads/main/openapi/formant-admin-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Formant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formant secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Formant
provider_slug: formant
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/formant-admin-api.yaml
  type: http
slug: formant-authentication
source_filename: formant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formant-admin-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/formant-admin-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formant/refs/heads/main/authentication/formant-authentication.yml
summary_line: http · 1 scheme
tags:
- Robotics
- Robot Fleet Management
- Teleoperation
- Observability
- Telemetry
- ROS
- ROS2
- Edge Devices
- Physical Operations
- Incident Management
- Industrial AI
- SCADA
- Predictive Maintenance
- Remote Monitoring
- Embedded Devices
---
