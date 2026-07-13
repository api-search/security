---
api_key_in: []
api_specs:
- filename: plausible-stats-openapi.yml
  format: yaml
  label: Plausible Stats API
  slug: stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-stats-openapi.yml
- filename: plausible-events-openapi.yml
  format: yaml
  label: Plausible Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-events-openapi.yml
- filename: plausible-sites-openapi.yml
  format: yaml
  label: Plausible Sites API
  slug: sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-sites-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Plausible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plausible secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plausible
provider_slug: plausible
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/plausible-sites-openapi.yml
  - openapi/plausible-stats-openapi.yml
  type: http
slug: plausible-authentication
source_filename: plausible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/plausible-sites-openapi.yml, openapi/plausible-stats-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/plausible-sites-openapi.yml\n  - openapi/plausible-stats-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/authentication/plausible-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Cookie-Free
- GDPR
- Open Source
- Privacy
- Web Analytics
---
