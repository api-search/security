---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hoursquare-attendance-api-openapi.yml
  format: yaml
  label: HourSquare Attendance API
  slug: hoursquare-attendance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-attendance-api-openapi.yml
- filename: hoursquare-employees-api-openapi.yml
  format: yaml
  label: HourSquare Employees API
  slug: hoursquare-employees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-employees-api-openapi.yml
- filename: hoursquare-me-api-openapi.yml
  format: yaml
  label: HourSquare Me API
  slug: hoursquare-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-me-api-openapi.yml
- filename: hoursquare-oauth-api-openapi.yml
  format: yaml
  label: HourSquare OAuth API
  slug: hoursquare-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-oauth-api-openapi.yml
auth_types: []
description: HourSquare uses OAuth 2.0 client‑credentials flow. A company API key (client ID and client secret) is exchanged at the token endpoint for a short‑lived Bearer token, which is then sent in the Authorization header on every request.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hoursquare Authentication
name_suffix: Authentication
oauth_flows: []
overview: HourSquare declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HourSquare
provider_slug: hoursquare
scheme_count: 1
schemes:
- evidence: The API uses the OAuth 2.0 client-credentials grant. Exchange the key for a short-lived access token at the token endpoint, then send that token as a Bearer header on every call.
  flows:
  - client_credentials
  how_to_obtain: An administrator creates a key in Hub › Settings › API & integrations, receiving a Client ID (e.g., hsq_k7Qm3xZp) and a client secret. The client ID and secret are sent to the token endpoint using HTTP Basic or form fields to obtain an access token.
  name: OAuth2
  scopes:
  - attendance.record
  - attendance.read
  - attendance.reports
  - employees.read
  - leave.read
  token_url: https://api.hoursquare.com/api/public/v1/oauth/token
  type: oauth2
slug: hoursquare-authentication
source_filename: hoursquare-authentication.yml
source_heading: Authentication Profile
source_url: https://hoursquare.com/developers/getting-started/
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hoursquare.com/developers/getting-started/\nsources:\n- https://hoursquare.com/developers/getting-started/\n- https://hoursquare.com/developers/authentication-and-scopes/\n- https://hoursquare.com/ka/developers/authentication-and-scopes/\n- https://hoursquare.com/tools/hr-setup-planner/\ndescription: HourSquare uses OAuth 2.0 client‑credentials flow. A company API key (client ID and client secret) is exchanged at the token endpoint\n  for a short‑lived Bearer token, which is then sent in the Authorization header on every request.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: The API uses the OAuth 2.0 client-credentials grant. Exchange the key for a short-lived access token at the token endpoint, then send\n    that token as a Bearer header on every call.\n  flows:\n  - client_credentials\n  token_url: https://api.hoursquare.com/api/public/v1/oauth/token\n  scopes:\n\
  \  - attendance.record\n  - attendance.read\n  - attendance.reports\n  - employees.read\n  - leave.read\n  how_to_obtain: An administrator creates a key in Hub › Settings › API & integrations, receiving a Client ID (e.g., hsq_k7Qm3xZp) and a client\n    secret. The client ID and secret are sent to the token endpoint using HTTP Basic or form fields to obtain an access token.\ndocs: https://hoursquare.com/developers/getting-started/\n"
source_yaml_url: https://artifacts.apis.io/hoursquare/authentication/hoursquare-authentication.yml
summary_line: 1 scheme
tags:
- Human Resources
- Payroll
- Time Tracking
- Workforce Management
- Software-as-a-Service
---
