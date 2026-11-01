---
anonymous_access: false
api_key_in: []
api_specs:
- filename: patchmon-scoped-api-hosts-api-openapi.yml
  format: yaml
  label: PatchMon Scoped API - Hosts API
  slug: patchmon-scoped-api-hosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/patchmon/openapi/patchmon-scoped-api-hosts-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: derived
name: Patchmon Authentication
name_suffix: Authentication
oauth_flows: []
overview: PatchMon declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: PatchMon
provider_slug: patchmon
scheme_count: 6
schemes:
- description: Basic Auth using API credentials (token_key:token_secret). Used for Scoped API and GetHomepage endpoints.
  name: basicAuth
  scheme: basic
  type: http
- description: Agent API ID (host api_id). Used with X-API-KEY for agent/integration endpoints.
  in: header
  name: X-API-ID
  scheme: apiKeyAuth
  type: apiKey
- description: Agent API key. Used with X-API-ID for agent/integration endpoints.
  in: header
  name: X-API-KEY
  scheme: apiKeySecret
  type: apiKey
- description: Auto-enrollment token key. Used with X-Auto-Enrollment-Secret.
  in: header
  name: X-Auto-Enrollment-Key
  scheme: autoEnrollmentKey
  type: apiKey
- description: Auto-enrollment token secret.
  in: header
  name: X-Auto-Enrollment-Secret
  scheme: autoEnrollmentSecret
  type: apiKey
- bearerFormat: JWT
  description: PatchMon user session token, sent as a Bearer token or in the token cookie set at login. Used by web UI endpoints.
  name: bearerAuth
  scheme: bearer
  type: http
slug: patchmon-authentication
source_filename: patchmon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: https://patchmon.net/docs/openapi.json\nschemes:\n  - type: http\n    scheme: basic\n    description: \"Basic Auth using API credentials (token_key:token_secret). Used for Scoped API and GetHomepage endpoints.\"\n    name: basicAuth\n  - type: apiKey\n    in: header\n    name: X-API-ID\n    description: \"Agent API ID (host api_id). Used with X-API-KEY for agent/integration endpoints.\"\n    scheme: apiKeyAuth\n  - type: apiKey\n    in: header\n    name: X-API-KEY\n    description: \"Agent API key. Used with X-API-ID for agent/integration endpoints.\"\n    scheme: apiKeySecret\n  - type: apiKey\n    in: header\n    name: X-Auto-Enrollment-Key\n    description: \"Auto-enrollment token key. Used with X-Auto-Enrollment-Secret.\"\n    scheme: autoEnrollmentKey\n  - type: apiKey\n    in: header\n    name: X-Auto-Enrollment-Secret\n    description: \"Auto-enrollment token secret.\"\n    scheme: autoEnrollmentSecret\n  - type: http\n\
  \    scheme: bearer\n    bearerFormat: JWT\n    description: \"PatchMon user session token, sent as a Bearer token or in the token cookie set at login. Used by web UI endpoints.\"\n    name: bearerAuth\n"
source_yaml_url: https://artifacts.apis.io/patchmon/authentication/patchmon-authentication.yml
summary_line: 6 schemes
tags:
- Company
- Patch Management
- Linux
- FreeBSD
- Windows
- Open Source
---
