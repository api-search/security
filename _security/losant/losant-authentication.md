---
api_key_in: []
api_specs:
- filename: losant-application-api-openapi.yml
  format: yaml
  label: Losant Application API
  slug: losant-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-application-api-openapi.yml
- filename: losant-device-api-openapi.yml
  format: yaml
  label: Losant Device API
  slug: losant-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-device-api-openapi.yml
- filename: losant-experience-api-openapi.yml
  format: yaml
  label: Losant Experience API
  slug: losant-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-experience-api-openapi.yml
- filename: losant-authentication-and-account-api-openapi.yml
  format: yaml
  label: Losant Authentication and Account API
  slug: losant-authentication-and-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-authentication-and-account-api-openapi.yml
- filename: losant-data-and-data-tables-api-openapi.yml
  format: yaml
  label: Losant Data and Data Tables API
  slug: losant-data-and-data-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-data-and-data-tables-api-openapi.yml
- filename: losant-edge-and-embedded-compute-api-openapi.yml
  format: yaml
  label: Losant Edge and Embedded Compute API
  slug: losant-edge-and-embedded-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-edge-and-embedded-compute-api-openapi.yml
- filename: losant-enterprise-instance-api-openapi.yml
  format: yaml
  label: Losant Enterprise Instance API
  slug: losant-enterprise-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-enterprise-instance-api-openapi.yml
- filename: losant-notebooks-api-openapi.yml
  format: yaml
  label: Losant Notebooks API
  slug: losant-notebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-notebooks-api-openapi.yml
- filename: losant-workflow-engine-api-openapi.yml
  format: yaml
  label: Losant Workflow Engine API
  slug: losant-workflow-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-workflow-engine-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Losant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Losant secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Losant
provider_slug: losant
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Losant uses JSON Web Tokens (JWTs) for authentication. Obtain a token via POST /auth/user, POST /auth/device, POST /applications/{applicationId}/tokens, or POST /me/tokens and pass it in the Authorization header as `Bearer <token>`.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/losant-application-api-openapi.yml
  - openapi/losant-auth-api-openapi.yml
  - openapi/losant-data-api-openapi.yml
  - openapi/losant-device-api-openapi.yml
  - openapi/losant-edge-api-openapi.yml
  - openapi/losant-experience-api-openapi.yml
  - openapi/losant-instance-api-openapi.yml
  - openapi/losant-notebook-api-openapi.yml
  - openapi/losant-workflow-api-openapi.yml
  type: http
slug: losant-authentication
source_filename: losant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/losant-application-api-openapi.yml, openapi/losant-auth-api-openapi.yml, openapi/losant-data-api-openapi.yml,\n  openapi/losant-device-api-openapi.yml, openapi/losant-edge-api-openapi.yml, openapi/losant-experience-api-openapi.yml,\n  openapi/losant-instance-api-openapi.yml, openapi/losant-notebook-api-openapi.yml, openapi/losant-workflow-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Losant uses JSON Web Tokens (JWTs) for authentication. Obtain a token via POST\n    /auth/user, POST /auth/device, POST /applications/{applicationId}/tokens, or POST /me/tokens\n    and pass it in the Authorization header as `Bearer <token>`.\n  sources:\n  - openapi/losant-application-api-openapi.yml\n  - openapi/losant-auth-api-openapi.yml\n  - openapi/losant-data-api-openapi.yml\n  - openapi/losant-device-api-openapi.yml\n  - openapi/losant-edge-api-openapi.yml\n\
  \  - openapi/losant-experience-api-openapi.yml\n  - openapi/losant-instance-api-openapi.yml\n  - openapi/losant-notebook-api-openapi.yml\n  - openapi/losant-workflow-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/authentication/losant-authentication.yml
summary_line: http · 1 scheme
tags:
- IoT
- Internet Of Things
- Devices
- Edge Compute
- Embedded
- MQTT
- Industrial IoT
- Telemetry
- Workflow Automation
- Visual Workflow Engine
- Dashboards
- Time Series
- Connected Products
- Enterprise
---
