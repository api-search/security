---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Microtechmd Authentication
name_suffix: Authentication
oauth_flows: []
overview: MicroTech Medical declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: MicroTech Medical
provider_slug: microtechmd
scheme_count: 0
schemes: []
slug: microtechmd-authentication
source_filename: microtechmd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: live extraction of the AiDEX API Platform SPA (https://aidexapi.microtechmd.com\n  app.js) — auth/console endpoints and request headers observed; no OpenAPI published\napi: AiDEX API Platform\nnotes: >-\n  The AiDEX API Platform is a self-service developer portal for accessing blood\n  glucose data resources from MicroTech Medical's AiDEX continuous glucose\n  monitoring (CGM) devices. Developers register an account, log in, and are\n  issued API credentials from the console. The console/session itself is guarded\n  by a bearer-style token carried in a \"wt-token\" request header. No public\n  OpenAPI or OAuth authorization-server metadata is served, so the profile below\n  is derived from observed platform endpoints rather than a machine-readable spec.\nsecurity_schemes:\n- id: developer-api-key\n  type: apiKey\n  in: header\n  description: >-\n    API key/credential issued to a registered developer from the console\n    (retrieved\
  \ via /api/platform/auth/key). Used to authenticate calls to the\n    AiDEX blood-glucose data API. Exact header/parameter name is not published.\n  evidence: https://aidexapi.microtechmd.com/api/platform/auth/key\n- id: console-session-token\n  type: apiKey\n  in: header\n  scheme_name: wt-token\n  description: >-\n    Bearer-style session token returned by developer login and sent in the\n    \"wt-token\" header for console management calls (change password, modify\n    developer info, query personal info, logout).\n  evidence: https://aidexapi.microtechmd.com/api/platform/auth/login\nobserved_endpoints:\n- POST /api/platform/auth/register   # developer registration\n- POST /api/platform/auth/login      # developer login -> wt-token session\n- GET  /api/platform/auth/key        # retrieve issued API key/credential\n- POST /api/platform/console/changePassword\n- POST /api/platform/console/modifyDevInfo\n- GET  /api/platform/console/queryPersonalInfo\n- POST /api/platform/console/logout\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microtechmd/refs/heads/main/authentication/microtechmd-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Healthcare
- Medical Devices
- Diabetes
- Glucose Monitoring
- Continuous Glucose Monitoring
- Blood Glucose Data
- API
---
