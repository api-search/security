---
api_key_in: []
api_specs:
- filename: trellix-epo-api-openapi.yml
  format: yaml
  label: Trellix ePO API
  slug: trellix-epo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-epo-api-openapi.yml
- filename: trellix-action-history-api-openapi.yml
  format: yaml
  label: Trellix Action History API
  slug: trellix-action-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-action-history-api-openapi.yml
- filename: trellix-affected-hosts-api-openapi.yml
  format: yaml
  label: Trellix Affected Hosts API
  slug: trellix-affected-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-affected-hosts-api-openapi.yml
- filename: trellix-alerts-api-openapi.yml
  format: yaml
  label: Trellix Alerts API
  slug: trellix-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-alerts-api-openapi.yml
- filename: trellix-detections-api-openapi.yml
  format: yaml
  label: Trellix Detections API
  slug: trellix-detections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-detections-api-openapi.yml
- filename: trellix-devices-api-openapi.yml
  format: yaml
  label: Trellix Devices API
  slug: trellix-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-devices-api-openapi.yml
- filename: trellix-epo-api-openapi.yml
  format: yaml
  label: Trellix Epo API
  slug: trellix-epo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-epo-api-openapi.yml
- filename: trellix-events-api-openapi.yml
  format: yaml
  label: Trellix Events API
  slug: trellix-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-events-api-openapi.yml
- filename: trellix-groups-api-openapi.yml
  format: yaml
  label: Trellix Groups API
  slug: trellix-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-groups-api-openapi.yml
- filename: trellix-queries-api-openapi.yml
  format: yaml
  label: Trellix Queries API
  slug: trellix-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-queries-api-openapi.yml
- filename: trellix-reactions-api-openapi.yml
  format: yaml
  label: Trellix Reactions API
  slug: trellix-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-reactions-api-openapi.yml
- filename: trellix-response-actions-api-openapi.yml
  format: yaml
  label: Trellix Response Actions API
  slug: trellix-response-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-response-actions-api-openapi.yml
- filename: trellix-searches-api-openapi.yml
  format: yaml
  label: Trellix Searches API
  slug: trellix-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-searches-api-openapi.yml
- filename: trellix-threats-api-openapi.yml
  format: yaml
  label: Trellix Threats API
  slug: trellix-threats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-threats-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trellix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trellix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trellix
provider_slug: trellix
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained through the client credentials flow with soc.act.tg scope. Credentials are generated through the Trellix EDR Credential Generator.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trellix-edr-openapi.yml
  - openapi/trellix-epo-saas-openapi.yml
  type: http
slug: trellix-authentication
source_filename: trellix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trellix-edr-openapi.yml, openapi/trellix-epo-saas-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained through the client credentials flow with soc.act.tg\n    scope. Credentials are generated through the Trellix EDR Credential Generator.\n  sources:\n  - openapi/trellix-edr-openapi.yml\n  - openapi/trellix-epo-saas-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/authentication/trellix-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Security
- Cybersecurity
- Endpoint Security
- Threat Detection
- Threat Intelligence
- XDR
---
