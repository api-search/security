---
api_key_in: []
api_specs:
- filename: plausible-customprops-api-openapi.yml
  format: yaml
  label: Plausible CustomProps API
  slug: plausible-customprops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-customprops-api-openapi.yml
- filename: plausible-events-api-openapi.yml
  format: yaml
  label: Plausible Events API
  slug: plausible-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-events-api-openapi.yml
- filename: plausible-goals-api-openapi.yml
  format: yaml
  label: Plausible Goals API
  slug: plausible-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-goals-api-openapi.yml
- filename: plausible-guests-api-openapi.yml
  format: yaml
  label: Plausible Guests API
  slug: plausible-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-guests-api-openapi.yml
- filename: plausible-query-api-openapi.yml
  format: yaml
  label: Plausible Query API
  slug: plausible-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-query-api-openapi.yml
- filename: plausible-sharedlinks-api-openapi.yml
  format: yaml
  label: Plausible SharedLinks API
  slug: plausible-sharedlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-sharedlinks-api-openapi.yml
- filename: plausible-sites-api-openapi.yml
  format: yaml
  label: Plausible Sites API
  slug: plausible-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-sites-api-openapi.yml
- filename: plausible-teams-api-openapi.yml
  format: yaml
  label: Plausible Teams API
  slug: plausible-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plausible/refs/heads/main/openapi/plausible-teams-api-openapi.yml
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
