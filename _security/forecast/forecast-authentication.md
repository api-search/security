---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Forecast Authentication
name_suffix: Authentication
oauth_flows: []
overview: forecast declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: forecast
provider_slug: forecast
scheme_count: 1
schemes:
- description: Per-integration API key generated in the Forecast Admin module (Admin -> API Keys -> Generate New API Key). Sent on every request. Grants full access to the account; treat like a password. Keys can be individually disabled or deleted if compromised.
  id: forecast_api_key
  in: header
  name: X-FORECAST-API-KEY
  required: true
  type: apiKey
slug: forecast-authentication
source_filename: forecast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/Forecast-it/API/blob/master/README.md\ndocs: https://support.forecast.app/hc/en-us/articles/33378026998289-Using-API-Keys\napi: Forecast API\nbase_url: https://api.forecast.it/api/v1/\nsummary: >-\n  Forecast uses a single static API-key scheme. Each integration is issued its\n  own API key from the Admin module and presents it on every request in the\n  X-FORECAST-API-KEY header over TLS. There is no OAuth 2.0, OpenID Connect, or\n  short-lived token flow. Keys grant full account access and can be disabled or\n  deleted from Admin if compromised.\nschemes:\n- id: forecast_api_key\n  type: apiKey\n  in: header\n  name: X-FORECAST-API-KEY\n  description: >-\n    Per-integration API key generated in the Forecast Admin module (Admin ->\n    API Keys -> Generate New API Key). Sent on every request. Grants full\n    access to the account; treat like a password. Keys can be individually\n    disabled or deleted\
  \ if compromised.\n  required: true\ntransport:\n  tls_required: true\n  notes: SSL only; all requests must be HTTPS.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nkey_management:\n  provisioning: Admin module, one key per integration recommended\n  rotation: supported (generate new key, disable/delete old)\n  revocation: supported (disable or delete key in Admin)\nnotes: >-\n  Forecast was acquired by Accelo (2025) and the forecast.app brand now\n  redirects to accelo.com, but the api.forecast.it API host and X-FORECAST-API-KEY\n  scheme remain live.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forecast/refs/heads/main/authentication/forecast-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Project Management
- Resource Management
- Professional Services Automation
- Time Tracking
- PSA
- API
---
