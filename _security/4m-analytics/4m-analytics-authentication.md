---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: 4M Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: 4M Analytics secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 4M Analytics
provider_slug: 4m-analytics
scheme_count: 1
schemes:
- data_scope: all projects or single folder
  expiration: optional per-key expiration date
  in: query
  name: wfsApiKey
  provisioning: admin-requested via Customer Success Manager, generated in 4Map
  scope: 4M WFS API (OGC Web Feature Service)
  sources:
  - docs
  type: apiKey
slug: 4m-analytics-authentication
source_filename: 4m-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://help.4manalytics.com/en/articles/11670237-how-to-generate-your-wfs-api-key-and-connect-to-your-gis-platform\ndocs: https://help.4manalytics.com/en/collections/3720127-api-and-integrations\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  notes: >-\n    The 4M WFS API authenticates with an API key. Keys are admin-gated: an\n    organization admin first requests API access from their 4M Customer Success\n    Manager, then generates a key inside the 4Map web application (initials menu\n    -> \"Generate API Key\"). A key carries an optional link name, an optional\n    expiration date, and a data scope (all projects across the organization, or a\n    single folder). Generating a key returns a WFS endpoint URL embedding the key\n    for direct use in a GIS client. The 4Map application itself is protected by\n    interactive user sign-in at https://4map.4manalytics.com/signin. No OpenAPI\n    securityScheme is\
  \ published, so this profile is captured from the provider\n    documentation rather than derived from a spec.\nschemes:\n- name: wfsApiKey\n  type: apiKey\n  in: query\n  scope: 4M WFS API (OGC Web Feature Service)\n  provisioning: admin-requested via Customer Success Manager, generated in 4Map\n  expiration: optional per-key expiration date\n  data_scope: all projects or single folder\n  sources:\n  - docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4m-analytics/refs/heads/main/authentication/4m-analytics-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Geospatial
- GIS
- Mapping
- Utilities
- Infrastructure
- Subsurface
- Location Intelligence
- AI
- Construction Technology
---
