---
api_key_in:
- header
api_specs:
- filename: vectranetworks-accounts-api-openapi.yml
  format: yaml
  label: Vectra AI Accounts API
  slug: vectranetworks-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-accounts-api-openapi.yml
- filename: vectranetworks-assignment-outcomes-api-openapi.yml
  format: yaml
  label: Vectra AI Assignment Outcomes API
  slug: vectranetworks-assignment-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-assignment-outcomes-api-openapi.yml
- filename: vectranetworks-assignments-api-openapi.yml
  format: yaml
  label: Vectra AI Assignments API
  slug: vectranetworks-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-assignments-api-openapi.yml
- filename: vectranetworks-detections-api-openapi.yml
  format: yaml
  label: Vectra AI Detections API
  slug: vectranetworks-detections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-detections-api-openapi.yml
- filename: vectranetworks-entities-api-openapi.yml
  format: yaml
  label: Vectra AI Entities API
  slug: vectranetworks-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-entities-api-openapi.yml
- filename: vectranetworks-events-api-openapi.yml
  format: yaml
  label: Vectra AI Events API
  slug: vectranetworks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-events-api-openapi.yml
- filename: vectranetworks-groups-api-openapi.yml
  format: yaml
  label: Vectra AI Groups API
  slug: vectranetworks-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-groups-api-openapi.yml
- filename: vectranetworks-health-api-openapi.yml
  format: yaml
  label: Vectra AI Health API
  slug: vectranetworks-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-health-api-openapi.yml
- filename: vectranetworks-hosts-api-openapi.yml
  format: yaml
  label: Vectra AI Hosts API
  slug: vectranetworks-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-hosts-api-openapi.yml
- filename: vectranetworks-lockdown-api-openapi.yml
  format: yaml
  label: Vectra AI Lockdown API
  slug: vectranetworks-lockdown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-lockdown-api-openapi.yml
- filename: vectranetworks-match-api-openapi.yml
  format: yaml
  label: Vectra AI Match API
  slug: vectranetworks-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-match-api-openapi.yml
- filename: vectranetworks-notes-api-openapi.yml
  format: yaml
  label: Vectra AI Notes API
  slug: vectranetworks-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-notes-api-openapi.yml
- filename: vectranetworks-proxies-api-openapi.yml
  format: yaml
  label: Vectra AI Proxies API
  slug: vectranetworks-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-proxies-api-openapi.yml
- filename: vectranetworks-search-api-openapi.yml
  format: yaml
  label: Vectra AI Search API
  slug: vectranetworks-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-search-api-openapi.yml
- filename: vectranetworks-tagging-api-openapi.yml
  format: yaml
  label: Vectra AI Tagging API
  slug: vectranetworks-tagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-tagging-api-openapi.yml
- filename: vectranetworks-threat-feeds-api-openapi.yml
  format: yaml
  label: Vectra AI Threat Feeds API
  slug: vectranetworks-threat-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-threat-feeds-api-openapi.yml
- filename: vectranetworks-users-api-openapi.yml
  format: yaml
  label: Vectra AI Users API
  slug: vectranetworks-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-users-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Vectranetworks Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Vectra AI secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Vectra AI
provider_slug: vectranetworks
scheme_count: 2
schemes:
- in: header
  name: VectraToken
  parameter: authorization
  sources:
  - openapi/vectranetworks-detect-v2.3-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{vectra_portal_url}/oauth2/token
  name: oauth2
  sources:
  - openapi/vectranetworks-rux-v3.3-openapi.yml
  type: oauth2
slug: vectranetworks-authentication
source_filename: vectranetworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vectranetworks-detect-v2.3-openapi.yml, openapi/vectranetworks-rux-v3.3-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: VectraToken\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/vectranetworks-detect-v2.3-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{vectra_portal_url}/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/vectranetworks-rux-v3.3-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/authentication/vectranetworks-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Cybersecurity
- Network Detection and Response
- Threat Detection
- Security Operations
- Artificial Intelligence
- SIEM
---
