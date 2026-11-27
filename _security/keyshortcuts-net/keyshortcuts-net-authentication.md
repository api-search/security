---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keyshortcuts-net-analytics-api-openapi.yml
  format: yaml
  label: KeyShortcuts Analytics API
  slug: keyshortcuts-net-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-analytics-api-openapi.yml
- filename: keyshortcuts-net-apps-api-openapi.yml
  format: yaml
  label: KeyShortcuts Apps API
  slug: keyshortcuts-net-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-apps-api-openapi.yml
- filename: keyshortcuts-net-comparison-api-openapi.yml
  format: yaml
  label: KeyShortcuts Comparison API
  slug: keyshortcuts-net-comparison-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-comparison-api-openapi.yml
- filename: keyshortcuts-net-copy-counts-api-openapi.yml
  format: yaml
  label: KeyShortcuts Copy Counts API
  slug: keyshortcuts-net-copy-counts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-copy-counts-api-openapi.yml
- filename: keyshortcuts-net-feedback-api-openapi.yml
  format: yaml
  label: KeyShortcuts Feedback API
  slug: keyshortcuts-net-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-feedback-api-openapi.yml
- filename: keyshortcuts-net-health-api-openapi.yml
  format: yaml
  label: KeyShortcuts Health API
  slug: keyshortcuts-net-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-health-api-openapi.yml
- filename: keyshortcuts-net-mcp-api-openapi.yml
  format: yaml
  label: KeyShortcuts MCP API
  slug: keyshortcuts-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-mcp-api-openapi.yml
- filename: keyshortcuts-net-outreach-api-openapi.yml
  format: yaml
  label: KeyShortcuts Outreach API
  slug: keyshortcuts-net-outreach-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-outreach-api-openapi.yml
- filename: keyshortcuts-net-pageviews-api-openapi.yml
  format: yaml
  label: KeyShortcuts Pageviews API
  slug: keyshortcuts-net-pageviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-pageviews-api-openapi.yml
- filename: keyshortcuts-net-personalized-api-openapi.yml
  format: yaml
  label: KeyShortcuts Personalized API
  slug: keyshortcuts-net-personalized-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-personalized-api-openapi.yml
- filename: keyshortcuts-net-reverse-lookup-api-openapi.yml
  format: yaml
  label: KeyShortcuts Reverse Lookup API
  slug: keyshortcuts-net-reverse-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-reverse-lookup-api-openapi.yml
- filename: keyshortcuts-net-schools-api-openapi.yml
  format: yaml
  label: KeyShortcuts Schools API
  slug: keyshortcuts-net-schools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-schools-api-openapi.yml
- filename: keyshortcuts-net-search-api-openapi.yml
  format: yaml
  label: KeyShortcuts Search API
  slug: keyshortcuts-net-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-search-api-openapi.yml
- filename: keyshortcuts-net-semantic-actions-api-openapi.yml
  format: yaml
  label: KeyShortcuts Semantic Actions API
  slug: keyshortcuts-net-semantic-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-semantic-actions-api-openapi.yml
- filename: keyshortcuts-net-sources-api-openapi.yml
  format: yaml
  label: KeyShortcuts Sources API
  slug: keyshortcuts-net-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-sources-api-openapi.yml
- filename: keyshortcuts-net-stack-export-api-openapi.yml
  format: yaml
  label: KeyShortcuts Stack Export API
  slug: keyshortcuts-net-stack-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-stack-export-api-openapi.yml
- filename: keyshortcuts-net-teams-api-openapi.yml
  format: yaml
  label: KeyShortcuts Teams API
  slug: keyshortcuts-net-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-teams-api-openapi.yml
- filename: keyshortcuts-net-translation-api-openapi.yml
  format: yaml
  label: KeyShortcuts Translation API
  slug: keyshortcuts-net-translation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keyshortcuts-net/openapi/keyshortcuts-net-translation-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: KeyShortcuts Authentication
name_suffix: Authentication
oauth_flows: []
overview: KeyShortcuts secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KeyShortcuts
provider_slug: keyshortcuts-net
scheme_count: 1
schemes:
- name: adminAccess
  scheme: bearer
  sources:
  - openapi/keyshortcuts-net-openapi.json
  type: http
slug: keyshortcuts-net-authentication
source_filename: keyshortcuts-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/keyshortcuts-net-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: adminAccess\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/keyshortcuts-net-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/keyshortcuts-net/authentication/keyshortcuts-net-authentication.yml
summary_line: http · 1 scheme
tags:
- Keyboard Shortcuts
- Productivity Tools
- Reference Guides
- Developer Resources
---
