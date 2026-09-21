---
anonymous_access: false
api_key_in: []
api_specs:
- filename: curatorsearch-openapi.json
  format: json
  label: CuratorSearch API
  slug: curatorsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curatorsearch/refs/heads/main/openapi/curatorsearch-openapi.json
auth_types:
- none
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Curatorsearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: CuratorSearch secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CuratorSearch
provider_slug: curatorsearch
scheme_count: 0
schemes: []
slug: curatorsearch-authentication
source_filename: curatorsearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: https://curatorsearch.com/developers\ndocs: https://curatorsearch.com/developers#access\nsummary:\n  types: [none]\n  public_access: keyless\n  api_key_in: []\n  oauth2_flows: []\nnote: >-\n  The public JSON API and the MCP server are keyless (no authentication key). The provider asks\n  callers to send a descriptive User-Agent header identifying their project, but this is a courtesy\n  request, not an enforced credential. The OpenAPI 3.1 contract declares no securitySchemes, matching\n  the keyless model. CORS is open. A separate keyed partner feed exists for bulk/scraping needs and is\n  granted on request (email support@curatorsearch.com, subject \"Partner feed\"); its credentials are\n  not publicly documented.\nschemes: []\npartner_feed:\n  gated: true\n  access: on request\n  contact: support@curatorsearch.com\n  note: Credentials and scheme not publicly documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curatorsearch/refs/heads/main/authentication/curatorsearch-authentication.yml
summary_line: none · 0 schemes
tags:
- agent-native
- MCP
- OpenAPI
- llms-txt
- Open Data
- Job
- Cultural Heritage
- Museums
- curatorial
- salary-transparency
- glam
- museum jobs
- Job Board
- Salaries
- Pay Transparency
- Datasets
- RSS
---
