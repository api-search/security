---
api_key_in: []
api_specs:
- filename: when-i-work-openapi.yml
  format: yaml
  label: When I Work API
  slug: when-i-work-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/when-i-work/refs/heads/main/openapi/when-i-work-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: When I Work Authentication
name_suffix: Authentication
oauth_flows: []
overview: When I Work secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: When I Work
provider_slug: when-i-work
scheme_count: 1
schemes:
- bearerFormat: JSON Web Token
  description: "Authentication with When I Work is based on a token model using [JSON Web Tokens](https://jwt.io/). First, you authenticate using a private developer key and the username and password of a When I Work user. Your developer key can be used like the following in the headers.\n```\ncurl -X POST \\\n  https://api.login.wheniwork.com/login \\\n  -H 'W-Key: <INSERT_DEVELOPER_KEY_HERE>' \\\n  -H 'content-type: ap"
  name: W-Token
  scheme: bearer
  sources:
  - openapi/when-i-work-openapi.yml
  type: http
slug: when-i-work-authentication
source_filename: when-i-work-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/when-i-work-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: W-Token\n  type: http\n  scheme: bearer\n  bearerFormat: JSON Web Token\n  description: |-\n    Authentication with When I Work is based on a token model using [JSON Web Tokens](https://jwt.io/). First, you authenticate using a private developer key and the username and password of a When I Work user. Your developer key can be used like the following in the headers.\n    ```\n    curl -X POST \\\n      https://api.login.wheniwork.com/login \\\n      -H 'W-Key: <INSERT_DEVELOPER_KEY_HERE>' \\\n      -H 'content-type: ap\n  sources:\n  - openapi/when-i-work-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/when-i-work/refs/heads/main/authentication/when-i-work-authentication.yml
summary_line: http · 1 scheme
tags:
- Employee Scheduling
- Workforce Management
- Time Tracking
- Time Clock
- Shift Management
- Attendance
- Team Messaging
- Hourly Workers
- Labor Forecasting
- HR
---
