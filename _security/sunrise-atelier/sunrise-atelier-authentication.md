---
api_key_in: []
api_specs:
- filename: sunrise-atelier-ip-api-openapi.yml
  format: yaml
  label: Sunrise Atelier Ip API
  slug: sunrise-atelier-ip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sunrise-atelier/refs/heads/main/openapi/sunrise-atelier-ip-api-openapi.yml
- filename: sunrise-atelier-timezone-api-openapi.yml
  format: yaml
  label: Sunrise Atelier Timezone API
  slug: sunrise-atelier-timezone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sunrise-atelier/refs/heads/main/openapi/sunrise-atelier-timezone-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sunrise Atelier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sunrise Atelier declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Sunrise Atelier
provider_slug: sunrise-atelier
scheme_count: 0
schemes: []
slug: sunrise-atelier-authentication
source_filename: sunrise-atelier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: 2026-07-21\nmethod: searched\nsource: https://sunrise.am/developer (published docs) + live probe 2026-07-21\nprovider: sunrise-atelier\nsummary: >-\n  The Sunrise.am World Time API is a fully public, keyless API. The developer\n  documentation states \"No API Key required - just start fetching\" and CORS is\n  enabled for direct browser access. No API key, token, OAuth, or other\n  credential is issued or accepted; the only stated requirement is an\n  attribution link back to Time.Now.\napis:\n- name: Sunrise.am World Time API\n  baseURL: https://time.now/developer/api\n  schemes: []\n  auth_required: false\n  notes: >-\n    Open/anonymous access. Requests over HTTPS only. Attribution to Time.Now\n    is requested (not technically enforced). Verified live 2026-07-21: requests\n    with no Authorization header return 200.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunrise-atelier/refs/heads/main/authentication/sunrise-atelier-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Time
- Timezone
- Astronomy
- Geolocation
- Sunrise
- Sunset
- Developer API
---
